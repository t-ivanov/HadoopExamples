* __Program Name__: TestDFSIO 
 
* __Description__: 
[TestDFSIO](http://www.michael-noll.com/blog/2011/04/09/benchmarking-and-stress-testing-an-hadoop-cluster-with-terasort-testdfsio-nnbench-mrbench/) is a HDFS benchmark included in Hadoop distributions. It is designed to stress test the storage I/O (read and write) capabilities of a cluster. In this way performance bottlenecks in network, hardware, OS and Hadoop setup can be found and fixed. The benchmark consists of two parts: TestDFSIO-write and TestDFSIO-read. The write program starts multiple map tasks with each task writing a separate HDFS file. The read program starts multiple map tasks with each task sequentially reading the previously written HDFS files and measuring the file size and the task execution time. The benchmark uses a single reduce task to measure and compute two performance metrics for each map task: Average I/O Rate and Throughput. Respectively, Equation 1 and Equation 2 illustrate how the two metrics are calculated with N as the total number of map tasks and the index i (0< i < N), identifying the individual tasks.  

Equation 1: Average I/O rate (N) = (∑_(i=1)^N▒rate(i) )/N  = (∑_(i=1)^N▒(file size(i))/(time(i)))/N

Equation 2: Throughput (N) = (∑_(i=1)^N▒〖file size(i)〗)/(∑_(i=1)^N▒〖time(i)〗)



* __Usage__: TestDFSIO [genericOptions] -read [-random | -backward | -skip [-skipSize Size]] | -write | -append | -clean [-compression codecClassName] [-nrFiles N] [-size Size[B|KB|MB|GB|TB]] [-resFile resultFileName] [-bufferSize Bytes]

* __Options__: TestDFSIO.1.7

__-read__: start the read workload

__-write__: start the write workload

__-clean__: delete the generated data

__-nrFiles__: number of read files/number of map tasks

__-size__: size of read file in MB

__-resFile__:

__-bufferSize__:


* __Sample Experiments__: 
 
$sudo yarn jar hadoop-mapreduce-client-jobclient-tests.jar TestDFSIO -write -nrFiles 10 -size 10MB


| Input Data Size | Operation  | Parameter  |Exec. Time |Throughput MB/Sec|Average IO Rate MB/Sec|IO Rate Standard Deviation |
|-----------------|------------|------------|-----------|-----------------|----------------------|---------------------------|
|         10MB 	  |   write    |-nrFiles 10 |   42.458  |        14.10    |            16.94     |              7.94         |
|         10MB 	  |   write    |-nrFiles 10 |   40.826  |        14.72    |            19.62     |             10.15         |
|         10MB 	  |   read     |-nrFiles 10 |   39.547  |       540.54    |            724.26    |            421.48         |
|         10MB 	  |   read     |-nrFiles 10 |   39.593  |       555.55    |            870.94    |            615.90         |
