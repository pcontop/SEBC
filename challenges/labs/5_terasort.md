[root@cluster2node2 ~]# time hadoop jar /opt/cloudera/parcels/CDH-5.9.1-1.cdh5.9.1.p0.4/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/neymar/tgen640 /user/neymar/tsort640m
17/04/13 17:17:45 INFO terasort.TeraSort: starting
17/04/13 17:17:48 INFO hdfs.DFSClient: Created token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@PCONTOP.ES, renewer=yarn, realUser=, issueDate=1492118268113, maxDate=1492723068113, sequenceNumber=2, masterKeyId=6 on ha-hdfs:nameservice1
17/04/13 17:17:48 INFO security.TokenCache: Got dt for hdfs://nameservice1; Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@PCONTOP.ES, renewer=yarn, realUser=, issueDate=1492118268113, maxDate=1492723068113, sequenceNumber=2, masterKeyId=6)
17/04/13 17:17:48 INFO input.FileInputFormat: Total input paths to process : 8
Spent 759ms computing base-splits.
Spent 9ms computing TeraScheduler splits.
Computing input splits took 771ms
Sampling 10 splits of 416
Making 12 from 100000 sampled records
Computing parititions took 1067ms
Spent 1841ms computing partitions.
17/04/13 17:17:49 INFO client.RMProxy: Connecting to ResourceManager at cluster2node1.compwire.local/192.168.100.171:8032
17/04/13 17:17:50 INFO mapreduce.JobSubmitter: number of splits:416
17/04/13 17:17:51 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492117290079_0002
17/04/13 17:17:51 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@PCONTOP.ES, renewer=yarn, realUser=, issueDate=1492118268113, maxDate=1492723068113, sequenceNumber=2, masterKeyId=6)
17/04/13 17:17:51 INFO impl.YarnClientImpl: Submitted application application_1492117290079_0002
17/04/13 17:17:51 INFO mapreduce.Job: The url to track the job: http://cluster2node1.compwire.local:8088/proxy/application_1492117290079_0002/
17/04/13 17:17:51 INFO mapreduce.Job: Running job: job_1492117290079_0002
17/04/13 17:18:08 INFO mapreduce.Job: Job job_1492117290079_0002 running in uber mode : false
17/04/13 17:18:08 INFO mapreduce.Job:  map 0% reduce 0%
17/04/13 17:18:25 INFO mapreduce.Job:  map 1% reduce 0%
17/04/13 17:18:28 INFO mapreduce.Job:  map 2% reduce 0%
17/04/13 17:18:30 INFO mapreduce.Job:  map 3% reduce 0%
17/04/13 17:18:31 INFO mapreduce.Job:  map 4% reduce 0%
17/04/13 17:18:33 INFO mapreduce.Job:  map 5% reduce 0%
17/04/13 17:18:39 INFO mapreduce.Job:  map 6% reduce 0%
17/04/13 17:18:41 INFO mapreduce.Job:  map 7% reduce 0%
17/04/13 17:18:42 INFO mapreduce.Job:  map 8% reduce 0%
17/04/13 17:18:43 INFO mapreduce.Job:  map 9% reduce 0%
17/04/13 17:18:50 INFO mapreduce.Job:  map 10% reduce 0%
17/04/13 17:18:51 INFO mapreduce.Job:  map 11% reduce 0%
17/04/13 17:18:53 INFO mapreduce.Job:  map 12% reduce 0%
17/04/13 17:18:56 INFO mapreduce.Job:  map 13% reduce 0%
17/04/13 17:18:59 INFO mapreduce.Job:  map 14% reduce 0%
17/04/13 17:19:09 INFO mapreduce.Job:  map 15% reduce 0%
17/04/13 17:19:14 INFO mapreduce.Job:  map 16% reduce 0%
17/04/13 17:19:16 INFO mapreduce.Job:  map 17% reduce 0%
17/04/13 17:19:21 INFO mapreduce.Job:  map 18% reduce 0%
17/04/13 17:19:22 INFO mapreduce.Job:  map 19% reduce 0%
17/04/13 17:19:26 INFO mapreduce.Job:  map 20% reduce 0%
17/04/13 17:19:27 INFO mapreduce.Job:  map 21% reduce 0%
17/04/13 17:19:31 INFO mapreduce.Job:  map 22% reduce 0%
17/04/13 17:19:33 INFO mapreduce.Job:  map 23% reduce 0%
17/04/13 17:19:36 INFO mapreduce.Job:  map 24% reduce 0%
17/04/13 17:19:39 INFO mapreduce.Job:  map 25% reduce 0%
17/04/13 17:19:40 INFO mapreduce.Job:  map 26% reduce 0%
17/04/13 17:19:44 INFO mapreduce.Job:  map 27% reduce 0%
17/04/13 17:19:48 INFO mapreduce.Job:  map 28% reduce 0%
17/04/13 17:19:49 INFO mapreduce.Job:  map 29% reduce 0%
17/04/13 17:19:51 INFO mapreduce.Job:  map 30% reduce 0%
17/04/13 17:19:55 INFO mapreduce.Job:  map 31% reduce 0%
17/04/13 17:19:57 INFO mapreduce.Job:  map 32% reduce 0%
17/04/13 17:20:03 INFO mapreduce.Job:  map 34% reduce 0%
17/04/13 17:20:13 INFO mapreduce.Job:  map 35% reduce 0%
17/04/13 17:20:19 INFO mapreduce.Job:  map 36% reduce 0%
17/04/13 17:20:22 INFO mapreduce.Job:  map 37% reduce 0%
17/04/13 17:20:24 INFO mapreduce.Job:  map 38% reduce 0%
17/04/13 17:20:25 INFO mapreduce.Job:  map 39% reduce 0%
17/04/13 17:20:31 INFO mapreduce.Job:  map 40% reduce 0%
17/04/13 17:20:32 INFO mapreduce.Job:  map 41% reduce 0%
17/04/13 17:20:33 INFO mapreduce.Job:  map 42% reduce 0%
17/04/13 17:20:37 INFO mapreduce.Job:  map 43% reduce 0%
17/04/13 17:20:40 INFO mapreduce.Job:  map 44% reduce 0%
17/04/13 17:20:43 INFO mapreduce.Job:  map 45% reduce 0%
17/04/13 17:20:44 INFO mapreduce.Job:  map 46% reduce 0%
17/04/13 17:20:48 INFO mapreduce.Job:  map 47% reduce 0%
17/04/13 17:20:49 INFO mapreduce.Job:  map 48% reduce 0%
17/04/13 17:20:52 INFO mapreduce.Job:  map 49% reduce 0%
17/04/13 17:20:55 INFO mapreduce.Job:  map 50% reduce 0%
17/04/13 17:20:57 INFO mapreduce.Job:  map 51% reduce 0%
17/04/13 17:21:09 INFO mapreduce.Job:  map 52% reduce 0%
17/04/13 17:21:12 INFO mapreduce.Job:  map 53% reduce 0%
17/04/13 17:21:13 INFO mapreduce.Job:  map 54% reduce 0%
17/04/13 17:21:19 INFO mapreduce.Job:  map 55% reduce 0%
17/04/13 17:21:21 INFO mapreduce.Job:  map 56% reduce 0%
17/04/13 17:21:24 INFO mapreduce.Job:  map 57% reduce 0%
17/04/13 17:21:27 INFO mapreduce.Job:  map 58% reduce 0%
17/04/13 17:21:29 INFO mapreduce.Job:  map 59% reduce 0%
17/04/13 17:21:32 INFO mapreduce.Job:  map 60% reduce 0%
17/04/13 17:21:36 INFO mapreduce.Job:  map 61% reduce 0%
17/04/13 17:21:37 INFO mapreduce.Job:  map 62% reduce 0%
17/04/13 17:21:40 INFO mapreduce.Job:  map 63% reduce 0%
17/04/13 17:21:44 INFO mapreduce.Job:  map 64% reduce 0%
17/04/13 17:21:45 INFO mapreduce.Job:  map 65% reduce 0%
17/04/13 17:21:49 INFO mapreduce.Job:  map 66% reduce 0%
17/04/13 17:21:51 INFO mapreduce.Job:  map 67% reduce 0%
17/04/13 17:21:53 INFO mapreduce.Job:  map 68% reduce 0%
17/04/13 17:21:56 INFO mapreduce.Job:  map 69% reduce 0%
17/04/13 17:22:02 INFO mapreduce.Job:  map 70% reduce 0%
17/04/13 17:22:07 INFO mapreduce.Job:  map 71% reduce 0%
17/04/13 17:22:11 INFO mapreduce.Job:  map 72% reduce 0%
17/04/13 17:22:17 INFO mapreduce.Job:  map 73% reduce 0%
17/04/13 17:22:19 INFO mapreduce.Job:  map 74% reduce 0%
17/04/13 17:22:22 INFO mapreduce.Job:  map 75% reduce 0%
17/04/13 17:22:25 INFO mapreduce.Job:  map 76% reduce 0%
17/04/13 17:22:28 INFO mapreduce.Job:  map 77% reduce 0%
17/04/13 17:22:32 INFO mapreduce.Job:  map 78% reduce 0%
17/04/13 17:22:35 INFO mapreduce.Job:  map 79% reduce 0%
17/04/13 17:22:36 INFO mapreduce.Job:  map 80% reduce 0%
17/04/13 17:22:37 INFO mapreduce.Job:  map 81% reduce 0%
17/04/13 17:22:43 INFO mapreduce.Job:  map 82% reduce 0%
17/04/13 17:22:44 INFO mapreduce.Job:  map 83% reduce 0%
17/04/13 17:22:46 INFO mapreduce.Job:  map 84% reduce 0%
17/04/13 17:22:48 INFO mapreduce.Job:  map 85% reduce 0%
17/04/13 17:22:52 INFO mapreduce.Job:  map 85% reduce 2%
17/04/13 17:22:53 INFO mapreduce.Job:  map 85% reduce 5%
17/04/13 17:22:56 INFO mapreduce.Job:  map 85% reduce 10%
17/04/13 17:22:57 INFO mapreduce.Job:  map 85% reduce 12%
17/04/13 17:22:58 INFO mapreduce.Job:  map 85% reduce 14%
17/04/13 17:22:59 INFO mapreduce.Job:  map 86% reduce 17%
17/04/13 17:23:03 INFO mapreduce.Job:  map 86% reduce 18%
17/04/13 17:23:08 INFO mapreduce.Job:  map 86% reduce 19%
17/04/13 17:23:11 INFO mapreduce.Job:  map 87% reduce 19%
17/04/13 17:23:13 INFO mapreduce.Job:  map 87% reduce 20%
17/04/13 17:23:15 INFO mapreduce.Job:  map 87% reduce 21%
17/04/13 17:23:16 INFO mapreduce.Job:  map 88% reduce 21%
17/04/13 17:23:17 INFO mapreduce.Job:  map 88% reduce 22%
17/04/13 17:23:22 INFO mapreduce.Job:  map 89% reduce 22%
17/04/13 17:23:26 INFO mapreduce.Job:  map 90% reduce 22%
17/04/13 17:23:29 INFO mapreduce.Job:  map 91% reduce 23%
17/04/13 17:23:35 INFO mapreduce.Job:  map 92% reduce 23%
17/04/13 17:23:38 INFO mapreduce.Job:  map 93% reduce 23%
17/04/13 17:23:43 INFO mapreduce.Job:  map 94% reduce 23%
17/04/13 17:23:46 INFO mapreduce.Job:  map 95% reduce 23%
17/04/13 17:23:47 INFO mapreduce.Job:  map 95% reduce 24%
17/04/13 17:23:50 INFO mapreduce.Job:  map 96% reduce 24%
17/04/13 17:23:54 INFO mapreduce.Job:  map 97% reduce 24%
17/04/13 17:23:57 INFO mapreduce.Job:  map 98% reduce 24%
17/04/13 17:24:10 INFO mapreduce.Job:  map 99% reduce 25%
17/04/13 17:24:15 INFO mapreduce.Job:  map 100% reduce 25%
17/04/13 17:24:20 INFO mapreduce.Job:  map 100% reduce 32%
17/04/13 17:24:22 INFO mapreduce.Job:  map 100% reduce 38%
17/04/13 17:24:23 INFO mapreduce.Job:  map 100% reduce 45%
17/04/13 17:24:24 INFO mapreduce.Job:  map 100% reduce 47%
17/04/13 17:24:25 INFO mapreduce.Job:  map 100% reduce 52%
17/04/13 17:24:26 INFO mapreduce.Job:  map 100% reduce 59%
17/04/13 17:24:27 INFO mapreduce.Job:  map 100% reduce 62%
17/04/13 17:24:28 INFO mapreduce.Job:  map 100% reduce 64%
17/04/13 17:24:29 INFO mapreduce.Job:  map 100% reduce 69%
17/04/13 17:24:32 INFO mapreduce.Job:  map 100% reduce 74%
17/04/13 17:24:33 INFO mapreduce.Job:  map 100% reduce 78%
17/04/13 17:24:34 INFO mapreduce.Job:  map 100% reduce 80%
17/04/13 17:24:35 INFO mapreduce.Job:  map 100% reduce 81%
17/04/13 17:24:36 INFO mapreduce.Job:  map 100% reduce 82%
17/04/13 17:24:37 INFO mapreduce.Job:  map 100% reduce 83%
17/04/13 17:24:38 INFO mapreduce.Job:  map 100% reduce 84%
17/04/13 17:24:40 INFO mapreduce.Job:  map 100% reduce 85%
17/04/13 17:24:41 INFO mapreduce.Job:  map 100% reduce 89%
17/04/13 17:24:42 INFO mapreduce.Job:  map 100% reduce 90%
17/04/13 17:24:43 INFO mapreduce.Job:  map 100% reduce 91%
17/04/13 17:24:44 INFO mapreduce.Job:  map 100% reduce 93%
17/04/13 17:24:45 INFO mapreduce.Job:  map 100% reduce 94%
17/04/13 17:24:47 INFO mapreduce.Job:  map 100% reduce 96%
17/04/13 17:24:49 INFO mapreduce.Job:  map 100% reduce 97%
17/04/13 17:24:50 INFO mapreduce.Job:  map 100% reduce 98%
17/04/13 17:24:52 INFO mapreduce.Job:  map 100% reduce 99%
17/04/13 17:24:56 INFO mapreduce.Job:  map 100% reduce 100%
17/04/13 17:24:57 INFO mapreduce.Job: Job job_1492117290079_0002 completed successfully
17/04/13 17:24:57 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2908916494
                FILE: Number of bytes written=5806319529
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553648672
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=1284
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=24
        Job Counters
                Launched map tasks=416
                Launched reduce tasks=12
                Data-local map tasks=413
                Rack-local map tasks=3
                Total time spent by all maps in occupied slots (ms)=4688618
                Total time spent by all reduces in occupied slots (ms)=1193530
                Total time spent by all map tasks (ms)=4688618
                Total time spent by all reduce tasks (ms)=1193530
                Total vcore-seconds taken by all map tasks=4688618
                Total vcore-seconds taken by all reduce tasks=1193530
                Total megabyte-seconds taken by all map tasks=4801144832
                Total megabyte-seconds taken by all reduce tasks=1222174720
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2843146699
                Input split bytes=48672
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2843146699
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =4992
                Failed Shuffles=0
                Merged Map outputs=4992
                GC time elapsed (ms)=82129
                CPU time spent (ms)=2490410
                Physical memory (bytes) snapshot=210595463168
                Virtual memory (bytes) snapshot=683152347136
                Total committed heap usage (bytes)=250622246912
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/04/13 17:24:57 INFO terasort.TeraSort: done

real    7m12.741s
user    0m14.275s
sys     0m0.757s
[root@cluster2node2 ~]#
