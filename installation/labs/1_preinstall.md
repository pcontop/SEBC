1.

[root@cluster2node1 cdh5.10.1]# sysctl vm.swappiness
vm.swappiness = 30

vi /usr/lib/tuned/virtual-guest/tuned.conf
#replaced vm.swappiness = 1

sysctl vm.swappiness=1
#for the 'live' value.

2.
[root@cluster2node5 ~]# df -h
Filesystem               Size  Used Avail Use% Mounted on
/dev/mapper/centos-root   36G  1.3G   35G   4% /
devtmpfs                 7.8G     0  7.8G   0% /dev
tmpfs                    7.8G     0  7.8G   0% /dev/shm
tmpfs                    7.8G  8.5M  7.8G   1% /run
tmpfs                    7.8G     0  7.8G   0% /sys/fs/cgroup
/dev/sda1                497M  169M  329M  34% /boot
tmpfs                    1.6G     0  1.6G   0% /run/user/0
[root@cluster2node5 ~]#


4.
Following the steps here to effectively disable transparent huge pages:

https://docs.mongodb.com/manual/tutorial/transparent-huge-pages/


[root@cluster2node1 ~]# cat /sys/kernel/mm/transparent_hugepage/enabled
always madvise [never]
[root@cluster2node1 ~]# cat /sys/kernel/mm/transparent_hugepage/defrag
always madvise [never]

5.
[root@cluster2node1 ~]# ip addr
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN qlen 1
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: ens160: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP qlen 1000
    link/ether 00:50:56:86:e9:4b brd ff:ff:ff:ff:ff:ff
    inet 192.168.100.171/24 brd 192.168.100.255 scope global ens160
       valid_lft forever preferred_lft forever
    inet6 fe80::250:56ff:fe86:e94b/64 scope link
       valid_lft forever preferred_lft forever

6.
[root@cluster2node1 ~]# getent hosts
127.0.0.1       localhost localhost.localdomain localhost4 localhost4.localdomain4
127.0.0.1       localhost localhost.localdomain localhost6 localhost6.localdomain6
192.168.100.171 cluster2node1.lab.local cluster2node1
192.168.100.176 cluster2node2.lab.local cluster2node2
192.168.100.173 cluster2node3.lab.local cluster2node3
192.168.100.174 cluster2node4.lab.local cluster2node4
192.168.100.175 cluster2node5.lab.local cluster2node5

7.
[root@cluster2node1 ~]# systemctl status nscd
Unit nscd.service could not be found.
[root@cluster2node1 ~]# yum -y install nscd
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.globo.com
 * extras: mirror.globo.com
 * updates: mirror.globo.com
Resolving Dependencies
There are unfinished transactions remaining. You might consider running yum-complete-transaction, or "yum-complete-transaction --cleanup-only" and "yum history redo last", first to finish them. If those don't work you'll have to try removing/installing packages by hand (maybe package-cleanup can help).
The program yum-complete-transaction is found in the yum-utils package.
--> Running transaction check
---> Package nscd.x86_64 0:2.17-157.el7_3.1 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

======================================================================================================
 Package            Arch                 Version                          Repository             Size
======================================================================================================
Installing:
 nscd               x86_64               2.17-157.el7_3.1                 updates               267 k

Transaction Summary
======================================================================================================
Install  1 Package

Total download size: 267 k
Installed size: 179 k
Downloading packages:
nscd-2.17-157.el7_3.1.x86_64.rpm                                               | 267 kB  00:00:00
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : nscd-2.17-157.el7_3.1.x86_64                                                       1/1
  Verifying  : nscd-2.17-157.el7_3.1.x86_64                                                       1/1

Installed:
  nscd.x86_64 0:2.17-157.el7_3.1

Complete!
[root@cluster2node1 ~]# systemctl start nscd
[root@cluster2node1 ~]# systemctl status
? cluster2node1.compwire.local
    State: running
     Jobs: 0 queued
   Failed: 0 units
    Since: Mon 2017-04-03 14:54:29 -03; 4min 48s ago
   CGroup: /
           +-1 /usr/lib/systemd/systemd --switched-root --system --deserialize 21
           +-user.slice
           ¦ +-user-0.slice
           ¦   +-session-1.scope
           ¦     +-2145 sshd: root@pts/0
           ¦     +-2149 -bash
           ¦     +-2231 systemctl status
           ¦     +-2232 systemctl status
           +-system.slice
             +-nscd.service
             ¦ +-2218 /usr/sbin/nscd
             +-tuned.service
             ¦ +-900 /usr/bin/python -Es /usr/sbin/tuned -l -P
             +-postfix.service
             ¦ +-1505 /usr/libexec/postfix/master -w
             ¦ +-1557 pickup -l -t unix -u
             ¦ +-1558 qmgr -l -t unix -u
             
            

[root@cluster2node1 ~]# systemctl enable nscd


8.

[root@cluster2node1 ~]# systemctl status ntpd
? ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; enabled; vendor preset: disabled)
   Active: active (running) since Mon 2017-04-03 14:54:31 -03; 13min ago
 Main PID: 659 (ntpd)
   CGroup: /system.slice/ntpd.service
           +-659 /usr/sbin/ntpd -u ntp:ntp -g

Apr 03 14:54:33 cluster2node1.compwire.local ntpd[659]: Listen normally on 4 ens160 192.168.100.1...23
Apr 03 14:54:33 cluster2node1.compwire.local ntpd[659]: new interface(s) found: waking up resolver
Apr 03 14:54:33 cluster2node1.compwire.local ntpd_intres[665]: DNS 0.centos.pool.ntp.org -> 201.49...5
Apr 03 14:54:33 cluster2node1.compwire.local ntpd_intres[665]: DNS 1.centos.pool.ntp.org -> 200.19...8
Apr 03 14:54:33 cluster2node1.compwire.local ntpd_intres[665]: DNS 2.centos.pool.ntp.org -> 200.16...8
Apr 03 14:54:35 cluster2node1.compwire.local ntpd[659]: Listen normally on 5 ens160 fe80::250:56f...23
Apr 03 14:54:35 cluster2node1.compwire.local ntpd[659]: new interface(s) found: waking up resolver
Apr 03 15:00:09 cluster2node1.compwire.local ntpd[659]: 0.0.0.0 c61c 0c clock_step -0.762805 s
Apr 03 15:00:08 cluster2node1.compwire.local ntpd[659]: 0.0.0.0 c614 04 freq_mode
Apr 03 15:00:09 cluster2node1.compwire.local ntpd[659]: 0.0.0.0 c618 08 no_sys_peer
Hint: Some lines were ellipsized, use -l to show in full.
