* __Program Name__: WordCount
 
* [__Source Code__] (https://github.com/apache/hadoop-common/blob/trunk/hadoop-mapreduce-project/hadoop-mapreduce-client/hadoop-mapreduce-client-jobclient/src/test/java/org/apache/hadoop/mapred/WordCount.java) 

* __Description__: 
[Wordcount](http://wiki.apache.org/hadoop/WordCount) is a standard micro-benchmark based on MapReduce job. It takes a text file as an input and counts how often each word occurs. Each mapper reads a line as an input and breaks it into words, which then is emitted as a key/value pair, consisting of the word and 1 for each occurrence. Each reducer sums the counts for each word and outputs a single key/value pair, consisting of the word and the sum of all word’s occurrences. The WordCount workload is mostly CPU bound. 

* __Usage__: sudo yarn jar hadoop-mapreduce-examples.jar wordcount <in <out

* __Options__:

 __m__: maps

 __r__: reduces

 __in__: HDFS path to the input files

 __out__: HDFS path to the output files


* __Sample Experiments__: sudo yarn jar hadoop-mapreduce-examples.jar wordcount /user/root/data /user/root/data_out

[Sample Text Data (in zip)] (http://www.gutenberg.org/files/4300/4300.zip)


| Input Data Size | Input directory  | Output directory | Maps Time | Reducers Time | Bytes Written | Bytes Read |
|-----------------|------------------|------------------|-----------|---------------|-----------|--------------|
|     4300.txt    | /user/root/data  |/user/root/data_out|  4249ms  |  3755ms       |  527547   |  1573079     |

