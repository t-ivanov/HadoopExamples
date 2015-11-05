# HadoopExamples

* List all available example programs: $yarn jar hadoop-mapreduce-examples.jar

* List all available tests programs: $yarn jar hadoop-mapreduce-client-jobclient-tests.jar

  * DFSCIOTest: Distributed i/o benchmark of libhdfs.

  *	DistributedFSCheck: Distributed checkup of the file system consistency.

  *	JHLogAnalyzer: Job History Log analyzer.

  * MRReliabilityTest: A program that tests the reliability of the MR framework by injecting faults/failures.
  
  *	NNdataGenerator: Generate the data to be used by NNloadGenerator
  
  *	NNloadGenerator: Generate load on Namenode using NN loadgenerator run WITHOUT MR
  
  *	NNloadGeneratorMR: Generate load on Namenode using NN loadgenerator run as MR job
  
  *	NNstructureGenerator: Generate the structure to be used by NNdataGenerator
  
  *	SliveTest: HDFS Stress Test and Live Data Verification.
  
  *	 fail: a job that always fails
  
  *	filebench: Benchmark SequenceFile(Input|Output)Format (block,record compressed and uncompressed), Text(Input|Output)Format (compressed and uncompressed).
  
  *	 largesorter: Large-Sort tester

  * loadgen: Generic map/reduce load generator
  
  *	mapredtest: A map/reduce test check.
  
  *	minicluster: Single process HDFS and MR cluster.
  
  *	mrbench: A map/reduce benchmark that can create many small jobs
  
  *	nnbench: A benchmark that stresses the namenode.
  
  * sleep: A job that sleeps at each map and reduce task.
	
  * testbigmapoutput: A map/reduce program that works on a very big non-splittable file and does identity map/reduce
  
  * testfilesystem: A test for FileSystem read/write.
  
  * testmapredsort: A map/reduce program that validates the map-reduce framework's sort.
  
  * testsequencefile: A test for flat files of binary key value pairs.	 
  
  * testsequencefileinputformat: A test for sequence file input format.

  * testtextinputformat: A test for text input format.
  
  * threadedmapbench: A map/reduce benchmark that compares the performance of maps with multiple spills over maps with 1 spill
 
[Hadoop exmaples source code] (https://github.com/apache/hadoop-common/tree/trunk/hadoop-mapreduce-project/hadoop-mapreduce-client/hadoop-mapreduce-client-jobclient/src/test/java/org/apache/hadoop/fs)
[Good tutorial on how to run the examples] (http://www.michael-noll.com/blog/2011/04/09/benchmarking-and-stress-testing-an-hadoop-cluster-with-terasort-testdfsio-nnbench-mrbench/)

Document Template
------------------------------
* Program Name: 
 
* Description:

What is the functionality of the program? Check the source code and use any available external resources (+references).

* Usage: 

Explain the input, output and additional config arguments given by the execution of the program. Give an example for a simple execution ($yarn jar hadoop-mapreduce-client-jobclient-tests.jar TestDFSIO -read -nrFiles 10 -fileSize 10). 

* Experimental Executions:


| input size | parameter 1 | ouput dir | Time Run1 | Time Run2 | Time Run3 | Avarega Time | SDV Time |
|-----------|------------|---------|---------|----------|----------|-------------|---------|
|            |             |           |           |           |           |              |          |

