[root@cluster2node1 ~]# sudo yum install mariadb-server
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.globo.com
 * extras: mirror.globo.com
 * updates: mirror.globo.com
Resolving Dependencies
There are unfinished transactions remaining. You might consider running yum-complete-transaction, or "yum-complete-transaction --cleanup-only" and "yum history redo last", first to finish them. If those don't work you'll have to try removing/installing packages by hand (maybe package-cleanup can help).
The program yum-complete-transaction is found in the yum-utils package.
--> Running transaction check
---> Package mariadb-server.x86_64 1:5.5.52-1.el7 will be installed
--> Processing Dependency: mariadb(x86-64) = 1:5.5.52-1.el7 for package: 1:mariadb-server-5.5.52-1.el7.x86_64
--> Processing Dependency: perl-DBI for package: 1:mariadb-server-5.5.52-1.el7.x86_64
--> Processing Dependency: perl-DBD-MySQL for package: 1:mariadb-server-5.5.52-1.el7.x86_64
--> Processing Dependency: perl(Data::Dumper) for package: 1:mariadb-server-5.5.52-1.el7.x86_64
--> Processing Dependency: perl(DBI) for package: 1:mariadb-server-5.5.52-1.el7.x86_64
--> Running transaction check
---> Package mariadb.x86_64 1:5.5.52-1.el7 will be installed
---> Package perl-DBD-MySQL.x86_64 0:4.023-5.el7 will be installed
---> Package perl-DBI.x86_64 0:1.627-4.el7 will be installed
--> Processing Dependency: perl(RPC::PlServer) >= 0.2001 for package: perl-DBI-1.627-4.el7.x86_64
--> Processing Dependency: perl(RPC::PlClient) >= 0.2000 for package: perl-DBI-1.627-4.el7.x86_64
---> Package perl-Data-Dumper.x86_64 0:2.145-3.el7 will be installed
--> Running transaction check
---> Package perl-PlRPC.noarch 0:0.2020-14.el7 will be installed
--> Processing Dependency: perl(Net::Daemon) >= 0.13 for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Test) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Log) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Compress::Zlib) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Running transaction check
---> Package perl-IO-Compress.noarch 0:2.061-2.el7 will be installed
--> Processing Dependency: perl(Compress::Raw::Zlib) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
--> Processing Dependency: perl(Compress::Raw::Bzip2) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
---> Package perl-Net-Daemon.noarch 0:0.48-5.el7 will be installed
--> Running transaction check
---> Package perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7 will be installed
---> Package perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

======================================================================================================
 Package                            Arch              Version                   Repository       Size
======================================================================================================
Installing:
 mariadb-server                     x86_64            1:5.5.52-1.el7            base             11 M
Installing for dependencies:
 mariadb                            x86_64            1:5.5.52-1.el7            base            8.7 M
 perl-Compress-Raw-Bzip2            x86_64            2.061-3.el7               base             32 k
 perl-Compress-Raw-Zlib             x86_64            1:2.061-4.el7             base             57 k
 perl-DBD-MySQL                     x86_64            4.023-5.el7               base            140 k
 perl-DBI                           x86_64            1.627-4.el7               base            802 k
 perl-Data-Dumper                   x86_64            2.145-3.el7               base             47 k
 perl-IO-Compress                   noarch            2.061-2.el7               base            260 k
 perl-Net-Daemon                    noarch            0.48-5.el7                base             51 k
 perl-PlRPC                         noarch            0.2020-14.el7             base             36 k

Transaction Summary
======================================================================================================
Install  1 Package (+9 Dependent packages)

Total download size: 21 M
Installed size: 107 M
Is this ok [y/d/N]: y
Downloading packages:
(1/10): perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64.rpm                         |  32 kB  00:00:00
(2/10): perl-Compress-Raw-Zlib-2.061-4.el7.x86_64.rpm                          |  57 kB  00:00:00
(3/10): perl-DBD-MySQL-4.023-5.el7.x86_64.rpm                                  | 140 kB  00:00:00
(4/10): perl-DBI-1.627-4.el7.x86_64.rpm                                        | 802 kB  00:00:00
(5/10): perl-Data-Dumper-2.145-3.el7.x86_64.rpm                                |  47 kB  00:00:00
(6/10): perl-IO-Compress-2.061-2.el7.noarch.rpm                                | 260 kB  00:00:00
(7/10): perl-Net-Daemon-0.48-5.el7.noarch.rpm                                  |  51 kB  00:00:00
(8/10): perl-PlRPC-0.2020-14.el7.noarch.rpm                                    |  36 kB  00:00:00
(9/10): mariadb-5.5.52-1.el7.x86_64.rpm                                        | 8.7 MB  00:00:02
(10/10): mariadb-server-5.5.52-1.el7.x86_64.rpm                                |  11 MB  00:00:08
------------------------------------------------------------------------------------------------------
Total                                                                 2.6 MB/s |  21 MB  00:00:08
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : perl-Data-Dumper-2.145-3.el7.x86_64                                               1/10
  Installing : perl-Net-Daemon-0.48-5.el7.noarch                                                 2/10
  Installing : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                       3/10
  Installing : 1:mariadb-5.5.52-1.el7.x86_64                                                     4/10
  Installing : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                        5/10
  Installing : perl-IO-Compress-2.061-2.el7.noarch                                               6/10
  Installing : perl-PlRPC-0.2020-14.el7.noarch                                                   7/10
  Installing : perl-DBI-1.627-4.el7.x86_64                                                       8/10
  Installing : perl-DBD-MySQL-4.023-5.el7.x86_64                                                 9/10
  Installing : 1:mariadb-server-5.5.52-1.el7.x86_64                                             10/10
  Verifying  : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                        1/10
  Verifying  : 1:mariadb-5.5.52-1.el7.x86_64                                                     2/10
  Verifying  : perl-Data-Dumper-2.145-3.el7.x86_64                                               3/10
  Verifying  : 1:mariadb-server-5.5.52-1.el7.x86_64                                              4/10
  Verifying  : perl-PlRPC-0.2020-14.el7.noarch                                                   5/10
  Verifying  : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                       6/10
  Verifying  : perl-Net-Daemon-0.48-5.el7.noarch                                                 7/10
  Verifying  : perl-DBI-1.627-4.el7.x86_64                                                       8/10
  Verifying  : perl-IO-Compress-2.061-2.el7.noarch                                               9/10
  Verifying  : perl-DBD-MySQL-4.023-5.el7.x86_64                                                10/10

Installed:
  mariadb-server.x86_64 1:5.5.52-1.el7

Dependency Installed:
  mariadb.x86_64 1:5.5.52-1.el7                     perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7
  perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7       perl-DBD-MySQL.x86_64 0:4.023-5.el7
  perl-DBI.x86_64 0:1.627-4.el7                     perl-Data-Dumper.x86_64 0:2.145-3.el7
  perl-IO-Compress.noarch 0:2.061-2.el7             perl-Net-Daemon.noarch 0:0.48-5.el7
  perl-PlRPC.noarch 0:0.2020-14.el7

Complete!
[root@cluster2node1 ~]# sudo service mariadb stop
Redirecting to /bin/systemctl stop  mariadb.service
[root@cluster2node1 ~]# mkdir backup
[root@cluster2node1 ~]# cp /var/lib/mysql/ib_logfile0 backup/ib_logfile0
cp: cannot stat ‘/var/lib/mysql/ib_logfile0’: No such file or directory
[root@cluster2node1 ~]# ls /etc/my.cnf
/etc/my.cnf

[root@cluster2node1 ~]# systemctl enable mariadb

[root@cluster2node1 mysql]# vi /etc/my.cnf
[root@cluster2node1 mysql]#  sudo service mariadb start
Redirecting to /bin/systemctl start  mariadb.service
[root@cluster2node1 mysql]# sudo /usr/bin/mysql_secure_installation

NOTE: RUNNING ALL PARTS OF THIS SCRIPT IS RECOMMENDED FOR ALL MariaDB
      SERVERS IN PRODUCTION USE!  PLEASE READ EACH STEP CAREFULLY!

In order to log into MariaDB to secure it, we'll need the current
password for the root user.  If you've just installed MariaDB, and
you haven't set the root password yet, the password will be blank,
so you should just press enter here.

Enter current password for root (enter for none):
OK, successfully used password, moving on...

Setting the root password ensures that nobody can log into the MariaDB
root user without the proper authorisation.

Set root password? [Y/n] y
New password:
Re-enter new password:
Password updated successfully!
Reloading privilege tables..
 ... Success!


By default, a MariaDB installation has an anonymous user, allowing anyone
to log into MariaDB without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.

Remove anonymous users? [Y/n]
 ... Success!

Normally, root should only be allowed to connect from 'localhost'.  This
ensures that someone cannot guess at the root password from the network.

Disallow root login remotely? [Y/n]
 ... Success!

By default, MariaDB comes with a database named 'test' that anyone can
access.  This is also intended only for testing, and should be removed
before moving into a production environment.

Remove test database and access to it? [Y/n]
 - Dropping test database...
 ... Success!
 - Removing privileges on test database...
 ... Success!

Reloading the privilege tables will ensure that all changes made so far
will take effect immediately.

Reload privilege tables now? [Y/n]
 ... Success!

Cleaning up...

All done!  If you've completed all of the above steps, your MariaDB
installation should now be secure.

Thanks for using MariaDB!
[root@cluster2node1 mysql]#
[root@cluster2node1 mysql]#


[root@cluster2node1 mysql]# cd
[root@cluster2node1 ~]# wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz
--2017-04-03 15:58:36--  https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz
Resolving dev.mysql.com (dev.mysql.com)... 137.254.60.11
Connecting to dev.mysql.com (dev.mysql.com)|137.254.60.11|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://cdn.mysql.com//Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz [following]
--2017-04-03 15:58:40--  https://cdn.mysql.com//Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz
Resolving cdn.mysql.com (cdn.mysql.com)... 23.32.33.62
Connecting to cdn.mysql.com (cdn.mysql.com)|23.32.33.62|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3923677 (3.7M) [application/x-tar-gz]
Saving to: ‘mysql-connector-java-5.1.41.tar.gz’

100%[==========================================================================================>] 3,923,677   8.96MB/s   in 0.4s

2017-04-03 15:58:40 (8.96 MB/s) - ‘mysql-connector-java-5.1.41.tar.gz’ saved [3923677/3923677]

[root@cluster2node1 ~]# ls
anaconda-ks.cfg  backup  CDH-5.10.1-1.cdh5.10.1.p0.10-el7.parcel.sha1  mysql-connector-java-5.1.41.tar.gz  test  var
[root@cluster2node1 ~]# tar -xf mysql-connector-java-5.1.41.tar.gz
[root@cluster2node1 ~]# ls
anaconda-ks.cfg  CDH-5.10.1-1.cdh5.10.1.p0.10-el7.parcel.sha1  mysql-connector-java-5.1.41.tar.gz  var
backup           mysql-connector-java-5.1.41                   test
[root@cluster2node1 ~]# cd mysql-connector-java-5.1.41
[root@cluster2node1 mysql-connector-java-5.1.41]# ls
build.xml  CHANGES  COPYING  docs  mysql-connector-java-5.1.41-bin.jar  README  README.txt  src
[root@cluster2node1 mysql-connector-java-5.1.41]# cp mysql-connector-java-5.1.41-bin.jar  /usr/share/java/mysql-connector-java.jar
cp: cannot create regular file ‘/usr/share/java/mysql-connector-java.jar’: No such file or directory
[root@cluster2node1 mysql-connector-java-5.1.41]# sudo mkdir -p /usr/share/java/
[root@cluster2node1 mysql-connector-java-5.1.41]# cp mysql-connector-java-5.1.41-bin.jar  /usr/share/java/mysql-connector-java.jar
[root@cluster2node1 mysql-connector-java-5.1.41]#


[root@cluster2node1 mysql-connector-java-5.1.41]# vi /etc/my.cnf
[root@cluster2node1 mysql-connector-java-5.1.41]# mysql -p root
Enter password:
ERROR 1049 (42000): Unknown database 'root'
[root@cluster2node1 mysql-connector-java-5.1.41]# mysql -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 11
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> GRANT REPLICATION SLAVE ON *.* TO replication_user;
Query OK, 0 rows affected (0.00 sec)

MariaDB [(none)]> FLUSH TABLES WITH READ LOCK;
Query OK, 0 rows affected (0.00 sec)

MariaDB [(none)]> SHOW MASTER STATUS
    -> ;
+-------------------------+----------+--------------+------------------+
| File                    | Position | Binlog_Do_DB | Binlog_Ignore_DB |
+-------------------------+----------+--------------+------------------+
| mysql_binary_log.000003 |     1610 |              |                  |
+-------------------------+----------+--------------+------------------+
1 row in set (0.00 sec)

MariaDB [(none)]>

[root@cluster2node1 ~]# mysqldump --all-databases -p > dump.sql
Enter password:
[root@cluster2node1 ~]# ls
anaconda-ks.cfg  CDH-5.10.1-1.cdh5.10.1.p0.10-el7.parcel.sha1  mysql-connector-java-5.1.41         test
backup           dump.sql                                      mysql-connector-java-5.1.41.tar.gz  var
[root@cluster2node1 ~]# less dump.sql
[root@cluster2node1 ~]# sftp cluster2node2
root@cluster2node2's password:
Connected to cluster2node2.
sftp> put dump.sql
Uploading dump.sql to /root/dump.sql
dump.sql                                                                                          100%  502KB 502.3KB/s   00:00
sftp> exit

[root@cluster2node2 ~]# mysql -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 10
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.
MariaDB [(none)]> source ~/dump.sql
Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 1 row affected (0.00 sec)

Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 39 rows affected (0.00 sec)
Records: 39  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 464 rows affected (0.01 sec)
Records: 464  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 1028 rows affected (0.01 sec)
Records: 1028  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 508 rows affected (0.02 sec)
Records: 508  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 2 rows affected (0.00 sec)
Records: 2  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.01 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 4 rows affected (0.00 sec)
Records: 4  Duplicates: 0  Warnings: 0

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

Query OK, 0 rows affected (0.00 sec)

MariaDB [mysql]>

# Added to master my.conf:
[mariadb]
log-bin
server_id=1
log-basename=master1

#Added to slave my.conf:
[mariadb]
server_id=2

[root@cluster2node1 ~]# mysql -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 15
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> GRANT REPLICATION SLAVE ON *.* TO 'root'@'cluster2node2.lab.local' identified by 'password';


MariaDB [(none)]> show master status;
+-------------------------+----------+--------------+------------------+
| File                    | Position | Binlog_Do_DB | Binlog_Ignore_DB |
+-------------------------+----------+--------------+------------------+
| mysql_binary_log.000003 |     3918 |              |                  |
+-------------------------+----------+--------------+------------------+


MariaDB [(none)]> UNLOCK TABLES;
Query OK, 0 rows affected (0.00 sec)

MariaDB [(none)]>


MariaDB [mysql]>

[root@cluster2node2 ~]# vi /etc/my.cnf
[root@cluster2node2 ~]# mysql -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 11
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.



Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]>   CHANGE MASTER TO
  MASTER_HOST='cluster2node1.lab.local',
  MASTER_USER='root',
  MASTER_PASSWORD='password',
  MASTER_PORT=3306,
  MASTER_LOG_FILE='master1-bin.000001',
  MASTER_LOG_POS=245,
  MASTER_CONNECT_RETRY=10;
Query OK, 0 rows affected (0.01 sec)

MariaDB [(none)]> start slave;
Query OK, 0 rows affected (0.00 sec)

MariaDB [(none)]> show slave status \G;
*************************** 1. row ***************************
               Slave_IO_State: Waiting for master to send event
                  Master_Host: cluster2node1.lab.local
                  Master_User: root
                  Master_Port: 3306
                Connect_Retry: 10
              Master_Log_File: master1-bin.000001
          Read_Master_Log_Pos: 881
               Relay_Log_File: mariadb-relay-bin.000002
                Relay_Log_Pos: 1167
        Relay_Master_Log_File: master1-bin.000001
             Slave_IO_Running: Yes
            Slave_SQL_Running: Yes
              Replicate_Do_DB:
          Replicate_Ignore_DB:
           Replicate_Do_Table:
       Replicate_Ignore_Table:
      Replicate_Wild_Do_Table:
  Replicate_Wild_Ignore_Table:
                   Last_Errno: 0
                   Last_Error:
                 Skip_Counter: 0
          Exec_Master_Log_Pos: 881
              Relay_Log_Space: 1463
              Until_Condition: None
               Until_Log_File:
                Until_Log_Pos: 0
           Master_SSL_Allowed: No
           Master_SSL_CA_File:
           Master_SSL_CA_Path:
              Master_SSL_Cert:
            Master_SSL_Cipher:
               Master_SSL_Key:
        Seconds_Behind_Master: 0
Master_SSL_Verify_Server_Cert: No
                Last_IO_Errno: 0
                Last_IO_Error:
               Last_SQL_Errno: 0
               Last_SQL_Error:
  Replicate_Ignore_Server_Ids:
             Master_Server_Id: 1
1 row in set (0.00 sec)

ERROR: No query specified

MariaDB [(none)]>
