# Hadoop Examples

* [Sample template] (https://github.com/t-ivanov/HadoopExamples/blob/master/Document_Template.md) that can be used when creating a workload description. 

* List all available __example__ programs: $yarn jar hadoop-mapreduce-examples.jar
  * __aggregatewordcount__: An Aggregate based map/reduce program that counts the words in the input files.
  
  * __aggregatewordhist__: An Aggregate based map/reduce program that computes the histogram of the words in the input files.
  
  * __bbp__: A map/reduce program that uses Bailey-Borwein-Plouffe to compute exact digits of Pi.

  * __dbcount__: An example job that count the pageview counts from a database.

  * __distbbp__: A map/reduce program that uses a BBP-type formula to compute exact bits of Pi.

  * __grep__: A map/reduce program that counts the matches of a regex in the input.

  * __join__: A job that effects a join over sorted, equally partitioned datasets
  
  * __multifilewc__: A job that counts words from several files.
  
  * __pentomino__: A map/reduce tile laying program to find solutions to pentomino problems.
  
  * __pi__: A map/reduce program that estimates Pi using a quasi-Monte Carlo method.
  
  * __randomtextwriter__: A map/reduce program that writes 10GB of random textual data per node.
  
  * __randomwriter__: A map/reduce program that writes 10GB of random data per node.
  
  * __secondarysort__: An example defining a secondary sort to the reduce.
  
  * __sort__: A map/reduce program that sorts the data written by the random writer.
  
  * [__sudoku__] (https://github.com/danielOrbegoso/HadoopExamples/blob/master/Sudoku.md): A sudoku solver.
  
  * __teragen__: Generate data for the terasort
  
  * __terasort__: Run the terasort
  
  * __teravalidate__: Checking results of terasort
  
  * [__wordcount__] (https://github.com/t-ivanov/HadoopExamples/blob/master/Wordcount.md): A map/reduce program that counts the words in the input files.
  
  * __wordmean__: A map/reduce program that counts the average length of the words in the input files.
  
  * __wordmedian__: A map/reduce program that counts the median length of the words in the input files.
  
  * __wordstandarddeviation__: A map/reduce program that counts the standard deviation of the length of the words in the input files.

* List all available __tests__ programs: $yarn jar hadoop-mapreduce-client-jobclient-tests.jar

  * [__TestDFSIO__](https://github.com/t-ivanov/HadoopExamples/blob/master/TestDFSIO.md): Distributed i/o benchmark.

  * __DFSCIOTest__: Distributed i/o benchmark of libhdfs.

  * __DistributedFSCheck__: Distributed checkup of the file system consistency.

  * __JHLogAnalyzer__: Job History Log analyzer.

  * __MRReliabilityTest__: A program that tests the reliability of the MR framework by injecting faults/failures.
  
  * __NNdataGenerator__: Generate the data to be used by NNloadGenerator
  
  * __NNloadGenerator__: Generate load on Namenode using NN loadgenerator run WITHOUT MR
  
  * __NNloadGeneratorMR__: Generate load on Namenode using NN loadgenerator run as MR job
  
  * __NNstructureGenerator__: Generate the structure to be used by NNdataGenerator
  
  * __SliveTest__: HDFS Stress Test and Live Data Verification.
  
  * __fail__: a job that always fails
  
  * __filebench__: Benchmark SequenceFile(Input|Output)Format (block,record compressed and uncompressed), Text(Input|Output)Format (compressed and uncompressed).
  
  * __largesorter__: Large-Sort tester

  * __loadgen__: Generic map/reduce load generator
  
  * __mapredtest__: A map/reduce test check.
  
  * __minicluster__: Single process HDFS and MR cluster.
  
  * __mrbench__: A map/reduce benchmark that can create many small jobs
  
  * __nnbench__: A benchmark that stresses the namenode.
  
  * __sleep__: A job that sleeps at each map and reduce task.
	
  * __testbigmapoutput__: A map/reduce program that works on a very big non-splittable file and does identity map/reduce
  
  * __testfilesystem__: A test for FileSystem read/write.
  
  * __testmapredsort__: A map/reduce program that validates the map-reduce framework's sort.
  
  * __testsequencefile__: A test for flat files of binary key value pairs.	 
  
  * __testsequencefileinputformat__: A test for sequence file input format.

  * __testtextinputformat__: A test for text input format.
  
  * __threadedmapbench__: A map/reduce benchmark that compares the performance of maps with multiple spills over maps with 1 spill
 
* [Hadoop exmaples source code] (https://github.com/apache/hadoop-common/tree/trunk/hadoop-mapreduce-project/hadoop-mapreduce-client/hadoop-mapreduce-client-jobclient/src/test/java/org/apache/hadoop/fs)

* [Good tutorial on how to run the examples] (http://www.michael-noll.com/blog/2011/04/09/benchmarking-and-stress-testing-an-hadoop-cluster-with-terasort-testdfsio-nnbench-mrbench/)

