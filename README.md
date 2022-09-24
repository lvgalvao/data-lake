# Data Lake

<img src="https://github.com/lvgalvao/data-lake/blob/main/src/picture2.png?raw=true" alt="DataLakeVsDataWaresouse" style="height: 400px; width:800px;"/>

### This repository aims to show some uses for a data lake, how is it different from a data warehouse, and the various options for implementing it on AWS

### Data Lakes, Why?
#### Q: Is there anything wrong with the data warehouse that we need something different?
R: No, data warehousing is a rather **mature field** with lots of cumulative experience over the years, **tried-and-true technologies. Dimensional modeling is still extremely relevant** to this day. **For many organizations, a data warehouse is still the best way to go**, perhaps, the biggest change would be going from an on-premise deployment to a cloud deployment.

#### Q: So, why do we need a data lake?
In recent years,** many factors drove the evolution of the data warehouse**, to name a few:
- The abundance of **unstructured data** (text, XML, JSON, logs, sensor data, images, voice, etc...) and unprecedented **data volumes**.
- The rise of **big data technologies like HDFS and Spark**.
- Types of analyses like predictive analytics based on machine learning and recommended systems and graph analytics drive data lake use.

#### Q: Can we have unstructured data in the data warehouse?
- Might be possible in the ETL process. For instance, we might be able to distill some elements from JSON data and put them in a tabular format.
- But later, we might decide that we want to transform it differently, so deciding on a particular form of transformation is **a strong commitment without enough knowledge**. E.g. we start by recording # of replies on a facebook of comments and then we are interested in the frequency of angry words.
- Some data is hard to put in a tabular format like **deep jsons structures**.
- Some data like text/pdf documents could be stored as **'blobs'** of data in a relational database but **useless unless processed to extract **metrics.

#### The Rise of Big Data Technologies
- The Hadoop file system (HDFS) made it possible to store Petabytes of data on commodity hardware. **Much lower cost per TB** compared to MPP databases.
- Associated processing tools starting from MapReduce, Pig, Hive, Impala, and Spark to name a few, made it possible to **process this data at scale on the same hardware used for storage.**
- It is possible to make data anlaysis without inserting it into a predefined schema. One can load a CSV file and make a query without creating a table, or inserting the data in the table. Similarly one can process unstructured text. This approach is known as **'Schema-on-read'**

#### New roles & Advanced Analytics
- The DW by design follows a** very well-architected** path to make a **clean, consistent and performant model** that business users can easily use to gain insights and make decisions.
- As data became an asset of the highest value (Data is the new oil), a role like the data scientist started to emerge seeking value from data.
- The data scientist job is almost impossible to conform to a **single rigid representation of data**. She needs freedom to represent data, join data sets together, retrieve new external data sources and more.
- The type of analytics such **machine learning, natural language, processing** need to access the raw data in forms totally different from a star-schema

#### The Data Lake is the new Data Warehouse
- The Data Lake shares the goals of the data warehouse of supporting business insights beyond the day-today transactional data handling.
The Data Lake is a new form of data warehouse that evolved to cope with:
- The **variety of data formats** and structuring
- The agile and ad-hoc nature of **data exploration** activities needed by new roles like tha data scientist
- The wide spectrum data transformation needed by advanced analytics like machine learning, graph analytics, and recommender systems.

#### Big Data Tech Effect #1: Low Cost

- 
### Big data technology Effect on Data Warehousing
#### - Project: Schema-on-read
#### - Project: Advanced Analytics

### Data Lakes, How?

### Big Data on AWS: The options
#### - Data Lakes S3+Spark(Local)
#### - Data Lakes S3+Spark(EMR)
#### - Data Lakes S3+Serverless(AWS Glue + Atlena)

### Data Lake Issues
