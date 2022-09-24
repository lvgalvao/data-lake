# Data Lake

### This repository aims to show some uses for a data lake, how is it different from a data warehouse and the various options for implamenting it on AWS

### Data Lakes, Why?
Q: Is there anything wrong with the data warehouse that we need something different?
R: No, data warehousing is a rather mature field with lots of cumulative experience over the years, tried-and-true technologies. Dimensional modelling is still extremely relevant to this day. For many organizations, a data warehouse is still the best way to go, perhaps, the biggest change would be going from an on-premise deployment to a cloud deployment.

Q: So, whey do we need a data lake?
In recent years, many factors drove the evolution of the data warehouse, to name a few:
- The abundance of unstructured data (text, xml, json, logs, sensor data, images, voice, etc...) and unprecendent data volumes;
- The rise of big data technologies like HDFS and Spark;
- Types of analyses like predictive analytics based on machine learning and recommended systems and graph analytics drive data lake use.

Q: Can we have unstractured data in the data warehouse?
- Might be possible in the ETL process. For instance, we might be able to distill some elements from json data and put in a tabular format.
- But later, we might decide that we want to transform it differently, so deciding on a particular form of transformations is <b>a strong commitment without enough knowledge</b>. E.g. we start by recording # of replies in a facebook of comments and then we are interested in the frequency of angry words.
- Some data is hard to put in a tabular format like deep jsons structures.
- Some data like text/pdf documents could be stored as 'blobs' of data in a relational database but totally useless unless processed to extract metrics.


### Big data technology Effect on Data Warehousing
#### - Project: Schema-on-read
#### - Project: Advanced Analytics

### Data Lakes, How?

### Big Data on AWS: The options
#### - Data Lakes S3+Spark(Local)
#### - Data Lakes S3+Spark(EMR)
#### - Data Lakes S3+Serverless(AWS Glue + Atlena)

### Data Lake Issues
