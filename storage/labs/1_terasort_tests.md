[root@cluster2node1 ~]# mkdir pcontop
[root@cluster2node1 ~]# useradd pcontop
[root@cluster2node1 ~]# su hdfs
[hdfs@cluster2node1 root]$ hdfs dfs -mkdir /user/pcontop
[hdfs@cluster2node1 root]$ hdfs dfs -chown pcontop /user/pcontop
[hdfs@cluster2node1 root]$ exit
exit
[root@cluster2node1 ~]# su pcontop
[pcontop@cluster2node1 root]$ hdfs dfs -ls
[pcontop@cluster2node1 root]$


[pcontop@cluster2node1 root]$ time hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar   teragen -D mapreduce.job.maps=4 -D dfs.block.size=33554432 100000000 /user/pcontop/teradataInput
17/04/04 19:18:57 INFO client.RMProxy: Connecting to ResourceManager at cluster2node1.compwire.local/192.168.100.171:8032
17/04/04 19:18:58 INFO terasort.TeraGen: Generating 100000000 using 4
17/04/04 19:18:58 INFO mapreduce.JobSubmitter: number of splits:4
17/04/04 19:18:58 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/04/04 19:18:59 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491331512753_0011
17/04/04 19:18:59 INFO impl.YarnClientImpl: Submitted application application_1491331512753_0011
17/04/04 19:18:59 INFO mapreduce.Job: The url to track the job: http://cluster2node1.compwire.local:8088/proxy/application_1491331512753_0011/
17/04/04 19:18:59 INFO mapreduce.Job: Running job: job_1491331512753_0011
17/04/04 19:19:12 INFO mapreduce.Job: Job job_1491331512753_0011 running in uber mode : false
17/04/04 19:19:12 INFO mapreduce.Job:  map 0% reduce 0%
17/04/04 19:19:31 INFO mapreduce.Job:  map 3% reduce 0%
17/04/04 19:19:32 INFO mapreduce.Job:  map 5% reduce 0%
17/04/04 19:19:34 INFO mapreduce.Job:  map 7% reduce 0%
17/04/04 19:19:35 INFO mapreduce.Job:  map 10% reduce 0%
17/04/04 19:19:38 INFO mapreduce.Job:  map 11% reduce 0%
17/04/04 19:19:39 INFO mapreduce.Job:  map 12% reduce 0%
17/04/04 19:19:41 INFO mapreduce.Job:  map 14% reduce 0%
17/04/04 19:19:42 INFO mapreduce.Job:  map 15% reduce 0%
17/04/04 19:19:44 INFO mapreduce.Job:  map 16% reduce 0%
17/04/04 19:19:45 INFO mapreduce.Job:  map 17% reduce 0%
17/04/04 19:19:47 INFO mapreduce.Job:  map 18% reduce 0%
17/04/04 19:19:48 INFO mapreduce.Job:  map 20% reduce 0%
17/04/04 19:19:49 INFO mapreduce.Job:  map 21% reduce 0%
17/04/04 19:19:50 INFO mapreduce.Job:  map 22% reduce 0%
17/04/04 19:19:53 INFO mapreduce.Job:  map 23% reduce 0%
17/04/04 19:19:54 INFO mapreduce.Job:  map 24% reduce 0%
17/04/04 19:19:55 INFO mapreduce.Job:  map 25% reduce 0%
17/04/04 19:19:56 INFO mapreduce.Job:  map 26% reduce 0%
17/04/04 19:19:59 INFO mapreduce.Job:  map 29% reduce 0%
17/04/04 19:20:01 INFO mapreduce.Job:  map 30% reduce 0%
17/04/04 19:20:04 INFO mapreduce.Job:  map 31% reduce 0%
17/04/04 19:20:06 INFO mapreduce.Job:  map 32% reduce 0%
17/04/04 19:20:14 INFO mapreduce.Job:  map 33% reduce 0%
17/04/04 19:20:18 INFO mapreduce.Job:  map 35% reduce 0%
17/04/04 19:20:20 INFO mapreduce.Job:  map 36% reduce 0%
17/04/04 19:20:23 INFO mapreduce.Job:  map 37% reduce 0%
17/04/04 19:20:24 INFO mapreduce.Job:  map 40% reduce 0%
17/04/04 19:20:25 INFO mapreduce.Job:  map 41% reduce 0%
17/04/04 19:20:29 INFO mapreduce.Job:  map 43% reduce 0%
17/04/04 19:20:30 INFO mapreduce.Job:  map 45% reduce 0%
17/04/04 19:20:31 INFO mapreduce.Job:  map 47% reduce 0%
17/04/04 19:20:35 INFO mapreduce.Job:  map 50% reduce 0%
17/04/04 19:20:36 INFO mapreduce.Job:  map 51% reduce 0%
17/04/04 19:20:37 INFO mapreduce.Job:  map 53% reduce 0%
17/04/04 19:20:41 INFO mapreduce.Job:  map 57% reduce 0%
17/04/04 19:20:43 INFO mapreduce.Job:  map 58% reduce 0%
17/04/04 19:20:48 INFO mapreduce.Job:  map 62% reduce 0%
17/04/04 19:20:50 INFO mapreduce.Job:  map 63% reduce 0%
17/04/04 19:20:54 INFO mapreduce.Job:  map 67% reduce 0%
17/04/04 19:20:56 INFO mapreduce.Job:  map 69% reduce 0%
17/04/04 19:21:00 INFO mapreduce.Job:  map 73% reduce 0%
17/04/04 19:21:02 INFO mapreduce.Job:  map 75% reduce 0%
17/04/04 19:21:08 INFO mapreduce.Job:  map 76% reduce 0%
17/04/04 19:21:14 INFO mapreduce.Job:  map 77% reduce 0%
17/04/04 19:21:18 INFO mapreduce.Job:  map 79% reduce 0%
17/04/04 19:21:20 INFO mapreduce.Job:  map 81% reduce 0%
17/04/04 19:21:24 INFO mapreduce.Job:  map 84% reduce 0%
17/04/04 19:21:26 INFO mapreduce.Job:  map 87% reduce 0%
17/04/04 19:21:30 INFO mapreduce.Job:  map 90% reduce 0%
17/04/04 19:21:32 INFO mapreduce.Job:  map 93% reduce 0%
17/04/04 19:21:36 INFO mapreduce.Job:  map 96% reduce 0%
17/04/04 19:21:38 INFO mapreduce.Job:  map 98% reduce 0%
17/04/04 19:21:40 INFO mapreduce.Job:  map 99% reduce 0%
17/04/04 19:21:41 INFO mapreduce.Job:  map 100% reduce 0%
17/04/04 19:21:47 INFO mapreduce.Job: Job job_1491331512753_0011 completed successfully
17/04/04 19:21:47 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=498804
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=344
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=16
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=8
        Job Counters
                Launched map tasks=4
                Other local map tasks=4
                Total time spent by all maps in occupied slots (ms)=579968
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=579968
                Total vcore-seconds taken by all map tasks=579968
                Total megabyte-seconds taken by all map tasks=593887232
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Input split bytes=344
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=2571
                CPU time spent (ms)=233490
                Physical memory (bytes) snapshot=993550336
                Virtual memory (bytes) snapshot=6275366912
                Total committed heap usage (bytes)=1073741824
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=214760662691937609
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=10000000000

real    2m54.909s
user    0m10.293s


[pcontop@cluster2node1 root]$ time hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/pcontop/teradataInput /user/pcontop/teradataOutput
17/04/04 18:56:56 INFO terasort.TeraSort: starting
17/04/04 18:56:59 INFO input.FileInputFormat: Total input paths to process : 4
Spent 383ms computing base-splits.
Spent 10ms computing TeraScheduler splits.
Computing input splits took 395ms
Sampling 10 splits of 300
Making 4 from 100000 sampled records
Computing parititions took 3047ms
Spent 3446ms computing partitions.
17/04/04 18:57:02 INFO client.RMProxy: Connecting to ResourceManager at cluster2node1.compwire.local/192.168.100.171:8032
17/04/04 18:57:04 INFO mapreduce.JobSubmitter: number of splits:300
17/04/04 18:57:04 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491331512753_0010
17/04/04 18:57:05 INFO impl.YarnClientImpl: Submitted application application_1491331512753_0010
17/04/04 18:57:05 INFO mapreduce.Job: The url to track the job: http://cluster2node1.compwire.local:8088/proxy/application_1491331512753_0010/
17/04/04 18:57:05 INFO mapreduce.Job: Running job: job_1491331512753_0010
17/04/04 18:57:15 INFO mapreduce.Job: Job job_1491331512753_0010 running in uber mode : false
17/04/04 18:57:15 INFO mapreduce.Job:  map 0% reduce 0%
17/04/04 18:57:30 INFO mapreduce.Job:  map 1% reduce 0%
17/04/04 18:57:31 INFO mapreduce.Job:  map 2% reduce 0%
17/04/04 18:57:44 INFO mapreduce.Job:  map 3% reduce 0%
17/04/04 18:57:46 INFO mapreduce.Job:  map 4% reduce 0%
17/04/04 18:58:00 INFO mapreduce.Job:  map 5% reduce 0%
17/04/04 18:58:10 INFO mapreduce.Job:  map 6% reduce 0%
17/04/04 18:58:20 INFO mapreduce.Job:  map 7% reduce 0%
17/04/04 18:58:28 INFO mapreduce.Job:  map 8% reduce 0%
17/04/04 18:58:38 INFO mapreduce.Job:  map 9% reduce 0%
17/04/04 18:58:45 INFO mapreduce.Job:  map 10% reduce 0%
17/04/04 18:58:56 INFO mapreduce.Job:  map 11% reduce 0%
17/04/04 18:58:59 INFO mapreduce.Job:  map 12% reduce 0%
17/04/04 18:59:19 INFO mapreduce.Job:  map 14% reduce 0%
17/04/04 18:59:33 INFO mapreduce.Job:  map 15% reduce 0%
17/04/04 18:59:36 INFO mapreduce.Job:  map 16% reduce 0%
17/04/04 18:59:48 INFO mapreduce.Job:  map 17% reduce 0%
17/04/04 18:59:50 INFO mapreduce.Job:  map 18% reduce 0%
17/04/04 19:00:01 INFO mapreduce.Job:  map 19% reduce 0%
17/04/04 19:00:16 INFO mapreduce.Job:  map 20% reduce 0%
17/04/04 19:00:25 INFO mapreduce.Job:  map 21% reduce 0%
17/04/04 19:00:30 INFO mapreduce.Job:  map 22% reduce 0%
17/04/04 19:00:43 INFO mapreduce.Job:  map 23% reduce 0%
17/04/04 19:00:44 INFO mapreduce.Job:  map 24% reduce 0%
17/04/04 19:00:57 INFO mapreduce.Job:  map 25% reduce 0%
17/04/04 19:00:59 INFO mapreduce.Job:  map 26% reduce 0%
17/04/04 19:01:18 INFO mapreduce.Job:  map 27% reduce 0%
17/04/04 19:01:23 INFO mapreduce.Job:  map 28% reduce 0%
17/04/04 19:01:33 INFO mapreduce.Job:  map 29% reduce 0%
17/04/04 19:01:41 INFO mapreduce.Job:  map 30% reduce 0%
17/04/04 19:01:50 INFO mapreduce.Job:  map 31% reduce 0%
17/04/04 19:01:55 INFO mapreduce.Job:  map 32% reduce 0%
17/04/04 19:02:10 INFO mapreduce.Job:  map 33% reduce 0%
17/04/04 19:02:13 INFO mapreduce.Job:  map 34% reduce 0%
17/04/04 19:02:24 INFO mapreduce.Job:  map 35% reduce 0%
17/04/04 19:02:30 INFO mapreduce.Job:  map 36% reduce 0%
17/04/04 19:02:42 INFO mapreduce.Job:  map 37% reduce 0%
17/04/04 19:02:46 INFO mapreduce.Job:  map 38% reduce 0%
17/04/04 19:02:56 INFO mapreduce.Job:  map 39% reduce 0%
17/04/04 19:03:08 INFO mapreduce.Job:  map 40% reduce 0%
17/04/04 19:03:18 INFO mapreduce.Job:  map 41% reduce 0%
17/04/04 19:03:24 INFO mapreduce.Job:  map 42% reduce 0%
17/04/04 19:03:35 INFO mapreduce.Job:  map 43% reduce 0%
17/04/04 19:03:39 INFO mapreduce.Job:  map 44% reduce 0%
17/04/04 19:03:49 INFO mapreduce.Job:  map 45% reduce 0%
17/04/04 19:03:54 INFO mapreduce.Job:  map 46% reduce 0%
17/04/04 19:04:10 INFO mapreduce.Job:  map 47% reduce 0%
17/04/04 19:04:13 INFO mapreduce.Job:  map 48% reduce 0%
17/04/04 19:04:23 INFO mapreduce.Job:  map 49% reduce 0%
17/04/04 19:04:32 INFO mapreduce.Job:  map 50% reduce 0%
17/04/04 19:04:41 INFO mapreduce.Job:  map 51% reduce 0%
17/04/04 19:04:46 INFO mapreduce.Job:  map 52% reduce 0%
17/04/04 19:04:55 INFO mapreduce.Job:  map 53% reduce 0%
17/04/04 19:05:00 INFO mapreduce.Job:  map 54% reduce 0%
17/04/04 19:05:16 INFO mapreduce.Job:  map 55% reduce 0%
17/04/04 19:05:23 INFO mapreduce.Job:  map 56% reduce 0%
17/04/04 19:05:33 INFO mapreduce.Job:  map 57% reduce 0%
17/04/04 19:05:38 INFO mapreduce.Job:  map 58% reduce 0%
17/04/04 19:05:45 INFO mapreduce.Job:  map 59% reduce 0%
17/04/04 19:05:53 INFO mapreduce.Job:  map 60% reduce 0%
17/04/04 19:06:01 INFO mapreduce.Job:  map 61% reduce 0%
17/04/04 19:06:14 INFO mapreduce.Job:  map 62% reduce 0%
17/04/04 19:06:21 INFO mapreduce.Job:  map 63% reduce 0%
17/04/04 19:06:28 INFO mapreduce.Job:  map 64% reduce 0%
17/04/04 19:06:35 INFO mapreduce.Job:  map 65% reduce 0%
17/04/04 19:06:44 INFO mapreduce.Job:  map 66% reduce 0%
17/04/04 19:06:48 INFO mapreduce.Job:  map 67% reduce 0%
17/04/04 19:06:57 INFO mapreduce.Job:  map 68% reduce 0%
17/04/04 19:07:11 INFO mapreduce.Job:  map 69% reduce 0%
17/04/04 19:07:21 INFO mapreduce.Job:  map 70% reduce 0%
17/04/04 19:07:27 INFO mapreduce.Job:  map 71% reduce 0%
17/04/04 19:07:35 INFO mapreduce.Job:  map 72% reduce 0%
17/04/04 19:07:40 INFO mapreduce.Job:  map 73% reduce 0%
17/04/04 19:07:50 INFO mapreduce.Job:  map 74% reduce 0%
17/04/04 19:07:58 INFO mapreduce.Job:  map 75% reduce 0%
17/04/04 19:08:12 INFO mapreduce.Job:  map 76% reduce 0%
17/04/04 19:08:15 INFO mapreduce.Job:  map 77% reduce 0%
17/04/04 19:08:28 INFO mapreduce.Job:  map 78% reduce 0%
17/04/04 19:08:33 INFO mapreduce.Job:  map 79% reduce 0%
17/04/04 19:08:42 INFO mapreduce.Job:  map 80% reduce 0%
17/04/04 19:08:51 INFO mapreduce.Job:  map 81% reduce 0%
17/04/04 19:09:00 INFO mapreduce.Job:  map 82% reduce 0%
17/04/04 19:09:10 INFO mapreduce.Job:  map 83% reduce 0%
17/04/04 19:09:17 INFO mapreduce.Job:  map 83% reduce 3%
17/04/04 19:09:25 INFO mapreduce.Job:  map 83% reduce 6%
17/04/04 19:09:26 INFO mapreduce.Job:  map 84% reduce 6%
17/04/04 19:09:29 INFO mapreduce.Job:  map 84% reduce 7%
17/04/04 19:09:30 INFO mapreduce.Job:  map 84% reduce 8%
17/04/04 19:09:35 INFO mapreduce.Job:  map 84% reduce 9%
17/04/04 19:09:36 INFO mapreduce.Job:  map 84% reduce 10%
17/04/04 19:09:39 INFO mapreduce.Job:  map 85% reduce 10%
17/04/04 19:09:41 INFO mapreduce.Job:  map 85% reduce 11%
17/04/04 19:09:43 INFO mapreduce.Job:  map 85% reduce 13%
17/04/04 19:09:49 INFO mapreduce.Job:  map 85% reduce 14%
17/04/04 19:09:55 INFO mapreduce.Job:  map 86% reduce 14%
17/04/04 19:10:19 INFO mapreduce.Job:  map 87% reduce 14%
17/04/04 19:10:25 INFO mapreduce.Job:  map 87% reduce 15%
17/04/04 19:10:32 INFO mapreduce.Job:  map 88% reduce 15%
17/04/04 19:10:41 INFO mapreduce.Job:  map 89% reduce 15%
17/04/04 19:10:50 INFO mapreduce.Job:  map 90% reduce 15%
17/04/04 19:11:11 INFO mapreduce.Job:  map 91% reduce 15%
17/04/04 19:11:22 INFO mapreduce.Job:  map 92% reduce 15%
17/04/04 19:11:36 INFO mapreduce.Job:  map 93% reduce 15%
17/04/04 19:11:43 INFO mapreduce.Job:  map 93% reduce 16%
17/04/04 19:11:47 INFO mapreduce.Job:  map 94% reduce 16%
17/04/04 19:11:57 INFO mapreduce.Job:  map 95% reduce 16%
17/04/04 19:12:15 INFO mapreduce.Job:  map 96% reduce 16%
17/04/04 19:12:29 INFO mapreduce.Job:  map 97% reduce 16%
17/04/04 19:12:44 INFO mapreduce.Job:  map 98% reduce 16%
17/04/04 19:12:57 INFO mapreduce.Job:  map 99% reduce 16%
17/04/04 19:13:02 INFO mapreduce.Job:  map 99% reduce 17%
17/04/04 19:13:11 INFO mapreduce.Job:  map 100% reduce 17%
17/04/04 19:13:25 INFO mapreduce.Job:  map 100% reduce 33%
17/04/04 19:13:29 INFO mapreduce.Job:  map 100% reduce 36%
17/04/04 19:13:31 INFO mapreduce.Job:  map 100% reduce 38%
17/04/04 19:13:33 INFO mapreduce.Job:  map 100% reduce 41%
17/04/04 19:13:35 INFO mapreduce.Job:  map 100% reduce 42%
17/04/04 19:13:37 INFO mapreduce.Job:  map 100% reduce 44%
17/04/04 19:13:40 INFO mapreduce.Job:  map 100% reduce 45%
17/04/04 19:13:42 INFO mapreduce.Job:  map 100% reduce 47%
17/04/04 19:13:44 INFO mapreduce.Job:  map 100% reduce 49%
17/04/04 19:13:46 INFO mapreduce.Job:  map 100% reduce 50%
17/04/04 19:13:48 INFO mapreduce.Job:  map 100% reduce 51%
17/04/04 19:13:50 INFO mapreduce.Job:  map 100% reduce 53%
17/04/04 19:13:52 INFO mapreduce.Job:  map 100% reduce 54%
17/04/04 19:13:54 INFO mapreduce.Job:  map 100% reduce 55%
17/04/04 19:13:56 INFO mapreduce.Job:  map 100% reduce 58%
17/04/04 19:14:00 INFO mapreduce.Job:  map 100% reduce 59%
17/04/04 19:14:06 INFO mapreduce.Job:  map 100% reduce 62%
17/04/04 19:14:07 INFO mapreduce.Job:  map 100% reduce 63%
17/04/04 19:14:12 INFO mapreduce.Job:  map 100% reduce 72%
17/04/04 19:14:14 INFO mapreduce.Job:  map 100% reduce 73%
17/04/04 19:14:18 INFO mapreduce.Job:  map 100% reduce 82%
17/04/04 19:14:20 INFO mapreduce.Job:  map 100% reduce 83%
17/04/04 19:14:24 INFO mapreduce.Job:  map 100% reduce 85%
17/04/04 19:14:26 INFO mapreduce.Job:  map 100% reduce 86%
17/04/04 19:14:29 INFO mapreduce.Job:  map 100% reduce 87%
17/04/04 19:14:30 INFO mapreduce.Job:  map 100% reduce 88%
17/04/04 19:14:35 INFO mapreduce.Job:  map 100% reduce 89%
17/04/04 19:14:36 INFO mapreduce.Job:  map 100% reduce 90%
17/04/04 19:14:41 INFO mapreduce.Job:  map 100% reduce 92%
17/04/04 19:14:42 INFO mapreduce.Job:  map 100% reduce 93%
17/04/04 19:14:47 INFO mapreduce.Job:  map 100% reduce 94%
17/04/04 19:14:48 INFO mapreduce.Job:  map 100% reduce 95%
17/04/04 19:14:53 INFO mapreduce.Job:  map 100% reduce 96%
17/04/04 19:14:54 INFO mapreduce.Job:  map 100% reduce 97%
17/04/04 19:14:59 INFO mapreduce.Job:  map 100% reduce 100%
17/04/04 19:15:08 INFO mapreduce.Job: Job job_1491331512753_0010 completed successfully
17/04/04 19:15:09 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=4458584131
                FILE: Number of bytes written=8839738316
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=10000043500
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=912
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=8
        Job Counters
                Launched map tasks=300
                Launched reduce tasks=4
                Data-local map tasks=298
                Rack-local map tasks=2
                Total time spent by all maps in occupied slots (ms)=3855423
                Total time spent by all reduces in occupied slots (ms)=873240
                Total time spent by all map tasks (ms)=3855423
                Total time spent by all reduce tasks (ms)=873240
                Total vcore-seconds taken by all map tasks=3855423
                Total vcore-seconds taken by all reduce tasks=873240
                Total megabyte-seconds taken by all map tasks=3947953152
                Total megabyte-seconds taken by all reduce tasks=894197760
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Map output bytes=10200000000
                Map output materialized bytes=4342801127
                Input split bytes=43500
                Combine input records=0
                Combine output records=0
                Reduce input groups=100000000
                Reduce shuffle bytes=4342801127
                Reduce input records=100000000
                Reduce output records=100000000
                Spilled Records=200000000
                Shuffled Maps =1200
                Failed Shuffles=0
                Merged Map outputs=1200
                GC time elapsed (ms)=46134
                CPU time spent (ms)=1881280
                Physical memory (bytes) snapshot=143998431232
                Virtual memory (bytes) snapshot=478698287104
                Total committed heap usage (bytes)=177691688960
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=10000000000
        File Output Format Counters
                Bytes Written=10000000000
17/04/04 19:15:09 INFO terasort.TeraSort: done

real    18m15.542s
user    0m23.084s
sys     0m1.857s