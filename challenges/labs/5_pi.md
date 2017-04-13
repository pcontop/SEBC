[root@cluster2node2 ~]# kinit ronaldo
Password for ronaldo@PCONTOP.ES:
[root@cluster2node2 ~]# hadoop jar /opt/cloudera/parcels/CDH-5.9.1-1.cdh5.9.1.p0.4/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 16 1000
Number of Maps  = 16
Samples per Map = 1000
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Starting Job
17/04/13 17:31:46 INFO client.RMProxy: Connecting to ResourceManager at cluster2node1.compwire.local/192.168.100.171:8032
17/04/13 17:31:47 INFO hdfs.DFSClient: Created token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@PCONTOP.ES, renewer=yarn, realUser=, issueDate=1492119107399, maxDate=1492723907399, sequenceNumber=3, masterKeyId=10 on ha-hdfs:nameservice1
17/04/13 17:31:47 INFO security.TokenCache: Got dt for hdfs://nameservice1; Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@PCONTOP.ES, renewer=yarn, realUser=, issueDate=1492119107399, maxDate=1492723907399, sequenceNumber=3, masterKeyId=10)
17/04/13 17:31:47 INFO input.FileInputFormat: Total input paths to process : 16
17/04/13 17:31:48 INFO mapreduce.JobSubmitter: number of splits:16
17/04/13 17:31:48 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492117290079_0003
17/04/13 17:31:48 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@PCONTOP.ES, renewer=yarn, realUser=, issueDate=1492119107399, maxDate=1492723907399, sequenceNumber=3, masterKeyId=10)
17/04/13 17:31:49 INFO impl.YarnClientImpl: Submitted application application_1492117290079_0003
17/04/13 17:31:49 INFO mapreduce.Job: The url to track the job: http://cluster2node1.compwire.local:8088/proxy/application_1492117290079_0003/
17/04/13 17:31:49 INFO mapreduce.Job: Running job: job_1492117290079_0003
17/04/13 17:32:00 INFO mapreduce.Job: Job job_1492117290079_0003 running in uber mode : false
17/04/13 17:32:00 INFO mapreduce.Job:  map 0% reduce 0%
17/04/13 17:32:22 INFO mapreduce.Job:  map 19% reduce 0%
17/04/13 17:32:25 INFO mapreduce.Job:  map 38% reduce 0%
17/04/13 17:32:26 INFO mapreduce.Job:  map 63% reduce 0%
17/04/13 17:32:27 INFO mapreduce.Job:  map 69% reduce 0%
17/04/13 17:32:28 INFO mapreduce.Job:  map 94% reduce 0%
17/04/13 17:32:29 INFO mapreduce.Job:  map 100% reduce 0%
17/04/13 17:32:35 INFO mapreduce.Job:  map 100% reduce 100%
17/04/13 17:32:36 INFO mapreduce.Job: Job job_1492117290079_0003 completed successfully
17/04/13 17:32:36 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=133
                FILE: Number of bytes written=2141013
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=4246
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=67
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=16
                Launched reduce tasks=1
                Data-local map tasks=16
                Total time spent by all maps in occupied slots (ms)=250001
                Total time spent by all reduces in occupied slots (ms)=4514
                Total time spent by all map tasks (ms)=250001
                Total time spent by all reduce tasks (ms)=4514
                Total vcore-seconds taken by all map tasks=250001
                Total vcore-seconds taken by all reduce tasks=4514
                Total megabyte-seconds taken by all map tasks=256001024
                Total megabyte-seconds taken by all reduce tasks=4622336
        Map-Reduce Framework
                Map input records=16
                Map output records=32
                Map output bytes=288
                Map output materialized bytes=544
                Input split bytes=2358
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=544
                Reduce input records=32
                Reduce output records=0
                Spilled Records=64
                Shuffled Maps =16
                Failed Shuffles=0
                Merged Map outputs=16
                GC time elapsed (ms)=946
                CPU time spent (ms)=15290
                Physical memory (bytes) snapshot=7496019968
                Virtual memory (bytes) snapshot=27149578240
                Total committed heap usage (bytes)=9213837312
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1888
        File Output Format Counters
                Bytes Written=97
Job Finished in 49.464 seconds
Estimated value of Pi is 3.14250000000000000000
[root@cluster2node2 ~]#
