
# That installls the correct maria db (5.5) for centos 7.
yum -y install mariadb-server

The hostname for the database is cluster2node1.compwire.local


[root@cluster2node5 mysql-connector-java-5.1.41]# mysql --version
mysql  Ver 15.1 Distrib 5.5.52-MariaDB, for Linux (x86_64) using readline 5.1
[root@cluster2node5 mysql-connector-java-5.1.41]# mysql -p
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 17
Server version: 5.5.52-MariaDB MariaDB Server

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hive               |
| hue                |
| mysql              |
| nava               |
| oozie              |
| performance_schema |
| rman               |
+--------------------+
9 rows in set (0.00 sec)

MariaDB [(none)]>

