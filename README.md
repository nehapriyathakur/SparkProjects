# SparkProjects
Five Projects for complete hands on with Spark and its APIs
1. Name: SparkKafkaConsumer
Details: Primary objective of this application is to develop a Spark Streaming application working as a Consumer to consume Kafka messages in real-time. Kafka Producer is supposed to produce CSV format data and will be transformed by Spark DataFrame APIs. A number of performance optimizations involved in transformation level e.g.repatitioning, broadcast joins orc file format etc..

2. Name: LogAnalysis
Details: Loganalysis is a Spark Streaming application to process production level server logs and harnesses the power of that data. After processing the resultant data can be used for various monitoring applications. Performance optimization techniques involved like caching, checkpointing to make the system fault-tolerant.
Format of data – The columns look like
ip datetime url response code content_size

a. Calculate statistics based on the content size.
b. Compute Response Code to Count- how many times response code appears
c. Any IPAddress that has accessed the server more than 10 times
d. 4 Top 10 Endpoints-traffic analysis

3. Name: CensusAnalytics
Details: This use case is to demonstrate the analytical insights of census data for countries like gender ratio. Certain key measures are taken care of in Spark configuration level to optimize the performance.

4. Name: Real Estate Analysis
Details: Based on historical real estate data various user queries can be addressed e.g.city wise price, property sale trends etc. using Spark.Using HDFS as input storage and processing those data with Spark Core with addressing key performance measures.
a. City wise list all the Condos which is not less than ten thousand
b. In GALT city which residential type has more than 800sq__ft. Display
their respective details street,sq__ft,sale_date,city 
c.  List top 5 residency details which lie in the budget of 60000-120000,
 an area more than 1150, sold after 17th may, min bedroom 3 and, min
bathroom 2.

5. Stock Analysis
StockAnalysis is a Spark application predominently using Spark SQL used to process Stock data and generate some useful insights from it e.g. average closing price,max and min closing price etc.We are providing Stock details in CSV format(can be downloaded from yahoo finance) to our application as input and reading them using Spark SQL with inbuilt CSV reader.Using various Spark transformations like join,orderBy,groupBy to generate all the required KPIs.Spark level performance optimizations involved like caching,ORC format,resource tuning etc.
a. The average closing price per year for Apple
b. The average closing price per month for Apple
c. When did the closing price for Apple go up or down by more than 2 dollars?
d. What was the max, min closing price for Apple and Google by Year?
e. Join Apple , Google, Microsoft, Amazon in order to compare closing
 Prices
f. Get year average closing prices for Apple , Google, Microsoft, Amazon


