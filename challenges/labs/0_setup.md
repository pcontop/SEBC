Cloud Providers: vShpere.
Nodes:
cluster2node1	192.168.100.171
cluster2node2	192.168.100.176
cluster2node3	192.168.100.173
cluster2node4	192.168.100.174
cluster2node5	192.168.100.175


[root@cluster2node1 ~]# df -k
Filesystem              1K-blocks    Used Available Use% Mounted on
/dev/mapper/centos-root  37173520 1302860  35870660   4% /
devtmpfs                  8123480       0   8123480   0% /dev
tmpfs                     8134176       0   8134176   0% /dev/shm
tmpfs                     8134176    8636   8125540   1% /run
tmpfs                     8134176       0   8134176   0% /sys/fs/cgroup
/dev/sda1                  508588  172496    336092  34% /boot
tmpfs                     1626836       0   1626836   0% /run/user/0
[root@cluster2node1 ~]#


[root@cluster2node2 ~]# df -k
Filesystem              1K-blocks    Used Available Use% Mounted on
/dev/mapper/centos-root  37173520 1169152  36004368   4% /
devtmpfs                  8123348       0   8123348   0% /dev
tmpfs                     8134044       0   8134044   0% /dev/shm
tmpfs                     8134044    8628   8125416   1% /run
tmpfs                     8134044       0   8134044   0% /sys/fs/cgroup
/dev/sda1                  508588  172496    336092  34% /boot
tmpfs                     1626812       0   1626812   0% /run/user/0
[root@cluster2node2 ~]#



[root@cluster2node3 ~]# df -k
Filesystem              1K-blocks    Used Available Use% Mounted on
/dev/mapper/centos-root  37173520 1169560  36003960   4% /
devtmpfs                  8123348       0   8123348   0% /dev
tmpfs                     8134044       0   8134044   0% /dev/shm
tmpfs                     8134044    8628   8125416   1% /run
tmpfs                     8134044       0   8134044   0% /sys/fs/cgroup
/dev/sda1                  508588  172496    336092  34% /boot
tmpfs                     1626812       0   1626812   0% /run/user/0
[root@cluster2node3 ~]#


[root@cluster2node4 ~]# df -k
Filesystem              1K-blocks    Used Available Use% Mounted on
/dev/mapper/centos-root  37173520 1169560  36003960   4% /
devtmpfs                  8123348       0   8123348   0% /dev
tmpfs                     8134044       0   8134044   0% /dev/shm
tmpfs                     8134044    8628   8125416   1% /run
tmpfs                     8134044       0   8134044   0% /sys/fs/cgroup
/dev/sda1                  508588  172496    336092  34% /boot
tmpfs                     1626812       0   1626812   0% /run/user/0
[root@cluster2node4 ~]#

[root@cluster2node5 ~]# df -k
Filesystem              1K-blocks    Used Available Use% Mounted on
/dev/mapper/centos-root  37173520 7200028  29973492  20% /
devtmpfs                  8123348       0   8123348   0% /dev
tmpfs                     8134044       0   8134044   0% /dev/shm
tmpfs                     8134044    8684   8125360   1% /run
tmpfs                     8134044       0   8134044   0% /sys/fs/cgroup
/dev/sda1                  508588  172496    336092  34% /boot
tmpfs                     1626812       0   1626812   0% /run/user/0
cm_processes              8134044       0   8134044   0% /run/cloudera-scm-agent/process
[root@cluster2node5 ~]#

[root@cluster2node1 ~]# yum repolist enabled
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: centos.xpg.com.br
 * extras: centos.xpg.com.br
 * updates: centos.xpg.com.br
repo id                                                  repo name                                                  status
!base/7/x86_64                                           CentOS-7 - Base                                            9,363
!extras/7/x86_64                                         CentOS-7 - Extras                                            311
!updates/7/x86_64                                        CentOS-7 - Updates                                         1,126
repolist: 10,800
[root@cluster2node1 ~]#

[root@cluster2node1 ~]# cat /etc/passwd | egrep 'neymar|ronaldo'
neymar:x:2010:2010::/home/neymar:/bin/bash
ronaldo:x:2016:2016::/home/ronaldo:/bin/bash

[root@cluster2node1 ~]# cat /etc/group | egrep 'barca|merengues'
barca:x:2017:ronaldo
merengues:x:2018:neymar


