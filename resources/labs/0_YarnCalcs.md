2. I altered the OS calculation to make it at most to 8 GB (and that's still a lot). My cluster will use Impala, so it's core uses have been calculated.
	Hbase will be on other cluster, so it's ok to not allocate resources to it.
3. It's a measure of how cpu bound the ccalculation is, with higher values being more cpu-bound. Lower values mean the number of drives are more of a factor in the limite of map and reducers.
 
