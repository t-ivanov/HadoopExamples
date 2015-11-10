* __Program Name__: WordCount
 
* __Description__: 
[Wordcount](http://wiki.apache.org/hadoop/WordCount) is a standard micro-benchmark based on MapReduce job. It takes a text file as an input and counts how often each word occurs. Each mapper reads a line as an input and breaks it into words, which then is emitted as a key/value pair, consisting of the word and 1 for each occurrence. Each reducer sums the counts for each word and outputs a single key/value pair, consisting of the word and the sum of all word’s occurrences. The WordCount workload is mostly CPU bound. 

* __Usage__: sudo yarn jar hadoop-mapreduce-examples.jar wordcount <in <out

* __Options__:

__in__: HDFS path to the input files

__out__: HDFS path to the output files



* __Sample Experiments__:




| Input Data Size | Parameter  | Output dir | Time Run1 | Time Run2 | Time Run3 | Average Time | Standard Deviation Time |
|-----------------|------------|-----------|-----------|-----------|-----------|--------------|----------|
|            	  |            |           |           |           |           |              |          |

