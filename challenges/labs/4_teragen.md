time hadoop jar /opt/cloudera/parcels/CDH-5.9.1-1.cdh5.9.1.p0.4/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D mapreduce.job.maps=8 -D dfs.blocksize=16000000 65536000 /user/neymar/tgen640

17/04/13 15:03:46 INFO client.RMProxy: Connecting to ResourceManager at cluster2node1.compwire.local/192.168.100.171:8032
17/04/13 15:03:47 INFO terasort.TeraSort: Generating 65536000 using 8
17/04/13 15:03:47 INFO mapreduce.JobSubmitter: number of splits:8
17/04/13 15:03:48 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492109274755_0001
17/04/13 15:03:48 INFO impl.YarnClientImpl: Submitted application application_1492109274755_0001
17/04/13 15:03:48 INFO mapreduce.Job: The url to track the job: http://cluster2node1.compwire.local:8088/proxy/application_1492109274755_0001/
17/04/13 15:03:48 INFO mapreduce.Job: Running job: job_1492109274755_0001
17/04/13 15:03:59 INFO mapreduce.Job: Job job_1492109274755_0001 running in uber mode : false
17/04/13 15:03:59 INFO mapreduce.Job:  map 0% reduce 0%
17/04/13 15:04:18 INFO mapreduce.Job:  map 1% reduce 0%
17/04/13 15:04:21 INFO mapreduce.Job:  map 2% reduce 0%
17/04/13 15:04:24 INFO mapreduce.Job:  map 3% reduce 0%
17/04/13 15:04:25 INFO mapreduce.Job:  map 4% reduce 0%
17/04/13 15:04:26 INFO mapreduce.Job:  map 6% reduce 0%
17/04/13 15:04:27 INFO mapreduce.Job:  map 7% reduce 0%
17/04/13 15:04:28 INFO mapreduce.Job:  map 8% reduce 0%
17/04/13 15:04:32 INFO mapreduce.Job:  map 9% reduce 0%
17/04/13 15:04:35 INFO mapreduce.Job:  map 10% reduce 0%
17/04/13 15:04:36 INFO mapreduce.Job:  map 12% reduce 0%
17/04/13 15:04:39 INFO mapreduce.Job:  map 14% reduce 0%
17/04/13 15:04:41 INFO mapreduce.Job:  map 15% reduce 0%
17/04/13 15:04:42 INFO mapreduce.Job:  map 16% reduce 0%
17/04/13 15:04:44 INFO mapreduce.Job:  map 17% reduce 0%
17/04/13 15:04:45 INFO mapreduce.Job:  map 19% reduce 0%
17/04/13 15:04:47 INFO mapreduce.Job:  map 20% reduce 0%
17/04/13 15:04:48 INFO mapreduce.Job:  map 22% reduce 0%
17/04/13 15:04:50 INFO mapreduce.Job:  map 23% reduce 0%
17/04/13 15:04:51 INFO mapreduce.Job:  map 25% reduce 0%
17/04/13 15:04:54 INFO mapreduce.Job:  map 26% reduce 0%
17/04/13 15:04:55 INFO mapreduce.Job:  map 28% reduce 0%
17/04/13 15:04:57 INFO mapreduce.Job:  map 29% reduce 0%
17/04/13 15:04:58 INFO mapreduce.Job:  map 31% reduce 0%
17/04/13 15:05:00 INFO mapreduce.Job:  map 32% reduce 0%
17/04/13 15:05:03 INFO mapreduce.Job:  map 33% reduce 0%
17/04/13 15:05:14 INFO mapreduce.Job:  map 35% reduce 0%
17/04/13 15:05:16 INFO mapreduce.Job:  map 36% reduce 0%
17/04/13 15:05:20 INFO mapreduce.Job:  map 38% reduce 0%
17/04/13 15:05:22 INFO mapreduce.Job:  map 39% reduce 0%
17/04/13 15:05:25 INFO mapreduce.Job:  map 40% reduce 0%
17/04/13 15:05:26 INFO mapreduce.Job:  map 42% reduce 0%
17/04/13 15:05:28 INFO mapreduce.Job:  map 43% reduce 0%
17/04/13 15:05:29 INFO mapreduce.Job:  map 45% reduce 0%
17/04/13 15:05:31 INFO mapreduce.Job:  map 46% reduce 0%
17/04/13 15:05:32 INFO mapreduce.Job:  map 47% reduce 0%
17/04/13 15:05:34 INFO mapreduce.Job:  map 48% reduce 0%
17/04/13 15:05:38 INFO mapreduce.Job:  map 49% reduce 0%
17/04/13 15:05:40 INFO mapreduce.Job:  map 50% reduce 0%
17/04/13 15:05:41 INFO mapreduce.Job:  map 52% reduce 0%
17/04/13 15:05:43 INFO mapreduce.Job:  map 53% reduce 0%
17/04/13 15:05:44 INFO mapreduce.Job:  map 55% reduce 0%
17/04/13 15:05:46 INFO mapreduce.Job:  map 56% reduce 0%
17/04/13 15:05:47 INFO mapreduce.Job:  map 58% reduce 0%
17/04/13 15:05:49 INFO mapreduce.Job:  map 59% reduce 0%
17/04/13 15:05:50 INFO mapreduce.Job:  map 61% reduce 0%
17/04/13 15:05:52 INFO mapreduce.Job:  map 62% reduce 0%
17/04/13 15:05:54 INFO mapreduce.Job:  map 64% reduce 0%
17/04/13 15:05:55 INFO mapreduce.Job:  map 65% reduce 0%
17/04/13 15:05:56 INFO mapreduce.Job:  map 66% reduce 0%
17/04/13 15:05:57 INFO mapreduce.Job:  map 67% reduce 0%
17/04/13 15:05:59 INFO mapreduce.Job:  map 68% reduce 0%
17/04/13 15:06:00 INFO mapreduce.Job:  map 69% reduce 0%
17/04/13 15:06:02 INFO mapreduce.Job:  map 70% reduce 0%
17/04/13 15:06:12 INFO mapreduce.Job:  map 71% reduce 0%
17/04/13 15:06:14 INFO mapreduce.Job:  map 72% reduce 0%
17/04/13 15:06:17 INFO mapreduce.Job:  map 73% reduce 0%
17/04/13 15:06:18 INFO mapreduce.Job:  map 74% reduce 0%
17/04/13 15:06:20 INFO mapreduce.Job:  map 76% reduce 0%
17/04/13 15:06:21 INFO mapreduce.Job:  map 77% reduce 0%
17/04/13 15:06:23 INFO mapreduce.Job:  map 79% reduce 0%
17/04/13 15:06:24 INFO mapreduce.Job:  map 80% reduce 0%
17/04/13 15:06:25 INFO mapreduce.Job:  map 81% reduce 0%
17/04/13 15:06:27 INFO mapreduce.Job:  map 82% reduce 0%
17/04/13 15:06:28 INFO mapreduce.Job:  map 83% reduce 0%
17/04/13 15:06:30 INFO mapreduce.Job:  map 85% reduce 0%
17/04/13 15:06:31 INFO mapreduce.Job:  map 86% reduce 0%
17/04/13 15:06:33 INFO mapreduce.Job:  map 88% reduce 0%
17/04/13 15:06:34 INFO mapreduce.Job:  map 89% reduce 0%
17/04/13 15:06:36 INFO mapreduce.Job:  map 90% reduce 0%
17/04/13 15:06:37 INFO mapreduce.Job:  map 91% reduce 0%
17/04/13 15:06:40 INFO mapreduce.Job:  map 92% reduce 0%
17/04/13 15:06:44 INFO mapreduce.Job:  map 93% reduce 0%
17/04/13 15:06:46 INFO mapreduce.Job:  map 94% reduce 0%
17/04/13 15:06:48 INFO mapreduce.Job:  map 95% reduce 0%
17/04/13 15:06:49 INFO mapreduce.Job:  map 96% reduce 0%
17/04/13 15:06:50 INFO mapreduce.Job:  map 97% reduce 0%
17/04/13 15:06:53 INFO mapreduce.Job:  map 98% reduce 0%
17/04/13 15:06:56 INFO mapreduce.Job:  map 99% reduce 0%
17/04/13 15:06:58 INFO mapreduce.Job:  map 100% reduce 0%
17/04/13 15:06:59 INFO mapreduce.Job: Job job_1492109274755_0001 completed successfully
17/04/13 15:06:59 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=981384
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=682
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=32
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=8
                Other local map tasks=8
                Total time spent by all maps in occupied slots (ms)=1328182
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=1328182
                Total vcore-seconds taken by all map tasks=1328182
                Total megabyte-seconds taken by all map tasks=1360058368
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=682
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=5484
                CPU time spent (ms)=308330
                Physical memory (bytes) snapshot=2258976768
                Virtual memory (bytes) snapshot=12708900864
                Total committed heap usage (bytes)=2598895616
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    3m16.150s
user    0m10.062s
sys     0m0.753s

[neymar@cluster2node2 root]$ hdfs dfs -ls /user/neymar/tgen640
Found 9 items
-rw-r--r--   3 neymar supergroup          0 2017-04-13 15:06 /user/neymar/tgen640/_SUCCESS
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00000
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00001
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00002
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00003
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00004
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00005
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00006
-rw-r--r--   3 neymar supergroup  819200000 2017-04-13 15:06 /user/neymar/tgen640/part-m-00007

[neymar@cluster2node2 root]$ hdfs fsck /user/neymar
Connecting to namenode via http://cluster2node1.compwire.local:50070
FSCK started by neymar (auth:SIMPLE) from /192.168.100.176 for path /user/neymar at Thu Apr 13 15:09:29 EDT 2017
.........Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    3
 Total files:   9
 Total symlinks:                0
 Total blocks (validated):      416 (avg. block size 15753846 B)
 Minimally replicated blocks:   416 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Thu Apr 13 15:09:29 EDT 2017 in 34 milliseconds


The filesystem under path '/user/neymar' is HEALTHY
