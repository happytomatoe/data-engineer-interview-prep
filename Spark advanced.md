1) What does [spark conf property] do?
A: https://spark.apache.org/docs/latest/configuration.html
2) How many partitions will be if we read 1GB file, 10 files which have 10 MB?
3) spark memory fraction
https://books.japila.pl/apache-spark-internals/configuration-properties/#sparkmemoryfraction
4) spark.sql.broadcast threshold - how size of the dataframe is calculated
https://kb.databricks.com/sql/bchashjoin-exceeds-bcjointhreshold-oom.html


5) How to investigate OOM?
6) What are the tools to get spark performance metrics/root cause of failure?
7) Spark garbage collection
8) Use of off-heap spark caching
The reasons to use off-heap memory rather than on-heap are the same as in all JVM-based applications. It helps to reduce GC overhead, to share some data among 2 different processes, to have always ready-to-use cache data (even after tasks restart). However, it doesn't come without costs. In the flip side, the off-heap increases CPU usage because of the extra translation from bytes of arrays into expected JVM object. The off-heap has also a trap. Even though we manage to store JVM objects off-heap, when they're read back to be used in the program, they can be allocated on-heap. Thus, there will be the need to garbage collect them. Therefore, in the Apache Spark context, in my opinion, it makes sense to use off-heap for SQL or Structured Streaming because they don't need to serialize back the data from the bytes array. The use in RDD-based programs can be useful though but should be studied with a little bit more care. Nonetheless, please notice that the Project Tungsten's format was designed to be efficient on on-heap memory too. Hence to decide whether go to on-heap or off-heap, we should always make the benchmark and use the most optimal solution only when the difference is big between them. Otherwise, it's always good to keep things simple and make them more complicated only when some important performance problems appear.
https://www.waitingforcode.com/apache-spark/apache-spark-off-heap-memory/read
9) 

