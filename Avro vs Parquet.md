AVRO vs. PARQUET
Read/Write Intensive & Query Pattern:
- AVRO is a row-based storage format, whereas PARQUET is a columnar-based storage format.
- PARQUET is much better for analytical querying, i.e., reads and querying are much more efficient than writing.
- Writiing operations in AVRO are better than in PARQUET.(why? becayse appending data to rows is easier than columns)
- PARQUET is ideal for querying a subset of columns in a multi-column table. AVRO is ideal in the case of ETL operations, where we need to query all the columns.
Compression:
- Columnar formats are better than row-based formats in terms of compression because storing the same type of values together allows more efficient compression. But currently snappy is not spltable
Schema evolution
- AVRO is much matured than PARQUET when it comes to schema evolution. PARQUET only supports schema append, whereas AVRO supports a much-featured schema evolution
, i.e., adding or modifying columns. And avro has backward, forward and full schema compatibility modes
Nested Columns
- If you have a lot of complex nested columns in your dataset and often only query a subset of the subcolumns, Parquet would be a good choice. Parquet is implemented using the record shredding and assembly algorithm described in the Dremel paper, which allows you to access and retrieve subcolumns without pulling the rest of the nested column.(https://towardsdatascience.com/demystify-hadoop-data-formats-avro-orc-and-parquet-e428709cf3bb)
Frameworks
- Spark provides great support for processing Parquet formats. Avro is often a good choice for Kafka.
[<img src="[http://www.google.com.au/images/nav_logo7.png](https://2s7gjr373w3x22jf92z99mgm5w-wpengine.netdna-ssl.com/wp-content/uploads/2018/05/Nexla-File-Format.png)">](http://google.com.au/)

[<img src="https://2s7gjr373w3x22jf92z99mgm5w-wpengine.netdna-ssl.com/wp-content/uploads/2018/05/Nexla-File-Format.png">](https://2s7gjr373w3x22jf92z99mgm5w-wpengine.netdna-ssl.com/wp-content/uploads/2018/05/Nexla-File-Format.png)
https://www.datanami.com/2018/05/16/big-data-file-formats-demystified/

Notes:
- Avro is a row-based data format slash a data serialization system released by Hadoop working group in 2009
- Parquet is a row columnar data format created by Cloudera and Twitter in 2013
