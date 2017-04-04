[root@cluster2node1 ~]# hdfs dfs -mkdir precious
mkdir: `precious': No such file or directory
[root@cluster2node1 ~]# su hdfs
[hdfs@cluster2node1 root]$ hdfs dfs -mkdir /user/root
[hdfs@cluster2node1 root]$ hdfs dfs -chown root /user/root
[hdfs@cluster2node1 root]$ exit
exit
[root@cluster2node1 ~]# hdfs dfs -mkdir precious
[root@cluster2node1 ~]# hdfs dfs -put "SEBC-master (1).zip"
put: unexpected URISyntaxException
[root@cluster2node1 ~]# hdfs dfs -put 'SEBC-master (1).zip' precious
put: unexpected URISyntaxException
[root@cluster2node1 ~]# mv 'SEBC-master (1).zip' 'SEBC-master.zip'
[root@cluster2node1 ~]# hdfs dfs -put 'SEBC-master.zip' precious
[root@cluster2node1 ~]# sudo -u hdfs hdfs dfsadmin -allowSnapshot /user/root/precious
Allowing snaphot on /user/root/precious succeeded
[root@cluster2node1 ~]# hdfs dfs -createSnapshot  /user/root/precious
Created snapshot /user/root/precious/.snapshot/s20170404-194841.954
[root@cluster2node1 ~]# hdfs dfs -rm /user/root/precious/*
17/04/04 19:49:46 INFO fs.TrashPolicyDefault: Moved: 'hdfs://cluster2node1.compwire.local:8020/user/root/precious/SEBC-master.zip' to trash at: hdfs://cluster2node1.compwire.local:8020/user/root/.Trash/Current/user/root/precious/SEBC-master.zip
[root@cluster2node1 ~]# hdfs dfs -lsr /user/root/precious/.snapshot
lsr: DEPRECATED: Please use 'ls -R' instead.
drwxr-xr-x   - root supergroup          0 2017-04-04 19:48 /user/root/precious/.snapshot/s20170404-194841.954
-rw-r--r--   3 root supergroup     473950 2017-04-04 19:46 /user/root/precious/.snapshot/s20170404-194841.954/SEBC-master.zip
[root@cluster2node1 ~]# hdfs dfs -ls -R /user/root/precious/.snapshot
drwxr-xr-x   - root supergroup          0 2017-04-04 19:48 /user/root/precious/.snapshot/s20170404-194841.954
-rw-r--r--   3 root supergroup     473950 2017-04-04 19:46 /user/root/precious/.snapshot/s20170404-194841.954/SEBC-master.zip
[root@cluster2node1 ~]# hdfs dfs -cp /user/root/precious/.snapshot/s20170404-194841.954/SEBC-master.zip /user/root/precious
[root@cluster2node1 ~]#