# Data Engineer Interview Preparation

Topics to cover:
- Java
1) https://www.amazon.com/Oracle-Certified-Professional-Programmer-Study/dp/1119584701
2) Functional interface - any interface with a SAM(Single Abstract Method) is a functional interface. @FunctinalInterface anotation tells compiler to check if this is the functional interface(https://docs.oracle.com/javase/8/docs/api/java/lang/FunctionalInterface.html)
3) streaming conepts in Java language, recommended book: Java 8 in Action: Lambdas, Streams, and Functional-Style Programming
4) code design concepts, recommended book: Java By Comparison, chapter 8: Let your data flow -> Side Effects
- Scala
5) https://docs.scala-lang.org/overviews/scala-book/introduction.html
6) [Scala udemy courses](https://www.udemy.com/course/stairway-to-scala-applied-part-1/)
<br />Most popular questions:
a) case classes
b) pattern matching
- SQL
6) https://www.essentialsql.com/
- https://towardsdatascience.com/sql-practical-details-cheat-sheet-for-data-analysis-f98406a71a09
- https://mode.com/sql-tutorial/sql-window-functions/
7) https://github.com/smpetersgithub/AdvancedSQLPuzzles
- Functional programming
8) https://docs.scala-lang.org/overviews/scala-book/functional-programming.html
- Distributed computing
- Spark
9) https://towardsdatascience.com/the-ultimate-guide-to-functional-programming-for-big-data-1e57b0d225a3
10) Joins - https://luminousmen.com/post/introduction-to-pyspark-join-types
- Yarn
11) Yarn schedulers - https://towardsdatascience.com/schedulers-in-yarn-concepts-to-configurations-5dd7ced6c214
-  Data Modeling (dimensional models and 3NF)
- Data storage formats(Parquet vs Avro)
1) https://www.clairvoyant.ai/blog/big-data-file-formats
2) https://www.adaltas.com/en/2020/07/23/benchmark-study-of-different-file-format/
3) https://luminousmen.com/post/big-data-file-formats
4) https://towardsdatascience.com/big-data-file-formats-explained-dfaabe9e8b33
5) [Parquet](https://github.com/happytomatoe/parquet-format)
6)  
- structured and semi-structured sources
- Big data architectures
- Cloud?
- Database&DWH
- Datalake vs Datawarehouse
12) CAP therorem - https://www.debadityachakravorty.com/system_design/captheorem/, https://softwaremill.com/how-to-choose-a-database-for-your-project/
13) How to choose a DB - https://en.pingcap.com/blog/how-to-efficiently-choose-the-right-database-for-your-applications/
14) Relation DB normalization - https://www.guru99.com/database-normalization.html
- SOLID
15) https://www.jrebel.com/blog/solid-principles-in-java
16) LSP - https://stackoverflow.com/questions/56860/what-is-an-example-of-the-liskov-substitution-principle

Helpfull resources:
1) https://www.startdataengineering.com/post/10-skills-to-ace-your-data-engineering-interview/
2) 

Notes:
- ETL vs ELT - looks like ELT is when data is extracted from source system, loaded into warehouse/object storage and transformed in data warehouse

Real life questions:
1) what is the file size you’ve used? Reason Behind your answer. 
2) How long does it take to run your script in production cluster? How did you optimized the timings. Challenges you have faced. 
3) what was the file size for production environment? 
4) Are you planning for anything to improve the performance? 
5) what size of file do you use for Development? 
6) what did you do to increase the performance(in your project's Hive, spark)? 
7) what is your cluster size? Reason Behind your answer. 
8) what are the challenges you have faced in your project? Give 2 examples? 
9) How to debug production issue?(logs, script counters, JVM) 
10) how do you select the eco-system tools for your project? 
11) How many nodes you are using currently? 
12) what is the job scheduler you use in production cluster? 
13) Each node size? Code storage location? 


TODO:
1) Add kafka
2) Add how to do performance optimizations for sql queries
3) Performance optimization for spark?
4) 


TODO: 
1) do a pentesting for existing knowledge - 
a) go through use cases for technologies 
