# Amazon EMR

## What is Amazon EMR?

Managed cluster platform that simplifies running big data frameworks.

- `Master Node`: A node that manages the cluster by running software components to coordinate the distribution of data and tasks among other nodes.
- `Core Node`: A node with software components that run tasks and store data in the Hadoop Distributed File System (HDFS) on your cluster. Multi-node clusters have at least one core node.
- `Taks Node`: A node with software components that only runs tasks and does not store data in HDFS task nodes are optional.

### Data Processing Frameworks

- Engine used to process and analyze data.
- Different frameworks are available for different kinds of processing needs,
- The main processing frameworks available for Amazon EMR are Hadoop MapReduce and Spark.

### Cluster Resource Management

- The resource management layer is responsible for managing cluster resources and scheduling the jobs for processing data.
- By default, Amazon EMR uses YARN (Yet Another Resource Negotiator).

### Storage

- Hadoop Distributed File System (HDFS) is a distributed, scalable file system for Hadoop.
- Using the EMR File System (EMRFS), Amazon EMR extends Hadoop to add the ability to directly access data stored in Amazon S3 as if it were a file system like HDFS.
- The local file system refers to a locally connected disk.

## Spark ETL

### What is Spark?

Apache Spark™ is a multi-language engine for executing data engineering, data science, and machine learning on single-node machines or clusters.

### In Memory Computing

Spark stores the data in the RAM of servers which allow quick access and in turn accelerates the speed of analytics.

### Faster Processing

Spark contains Resilient Distributed Dataset (RDD) which saves time in reading and writing operations, allowing it to run almost ten to one hundred times faster than Hadoop.

### Flexibility

Apache Spark supports multiple languages and allows the developers to write applications in Java, Scala, R, or Python.

## Hive

### What is Hive?

The Apache Hive™ data warehouse software facilitates reading, writing, and managing large datasets residing in distributed storage using SQL. Structure can be projected onto data already in storage. A command line tool and JDBC driver are provided to connect users to Hive.

### SQL Like Interface

Hive provides the necessary SQL abstraction to integrate SQL-like queries (HiveQL) into the underlying Java without the need to implement queries in the low-level Java API.

### Storage

Different storage types such as plain text, RCFile, HBase, ORC, and others.

## PIG

### What is PIG?

Apache PIG is a platform for analyzing large data sets that consists of a high-level language for expressing data analysis programs, coupled with infrastructure for evaluating these programs. The salient property of PIG programs is that their structure is amenable to substantial parallelization, which in turns enables them to handle very large data sets.

### How Does It Work?

It is an abstraction of Map Reduce which integrates with the lower level Java API which means parallel processing is easily achieved.

### Storage

Different storage types such as plain text, RCFile, HBase, ORC, and others.

## Amazon EMR Autoscaling

### What is Autoscaling?

Autoscaling is a cloud computing feature that enables organizations to scale cloud services such as server capacities or virtual machines up or down automatically, based on defined situations such as traffic or utilization levels.

### How does it work?

Autoscaling policies are added to an Amazon EMR cluster which define how nodes should be added or removed. There are options in terms of available RAM, disc, app running, apps pending, etc.

## Resources

- [ETL on Amazon EMR Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/c86bd131-f6bf-4e8f-b798-58fd450d3c44/en-US)
- [Amazon EMR - AWS EMR Tutorial - Full Course in 60 mins](https://www.youtube.com/watch?v=v9nk6mVxJDU)
- [Amazon EMR on EKS](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/emr-eks.html)
- [Amazon EMR vs Google Dataproc: Which is Better in 2022](https://gcpfirebase.com/amazon-emr-vs-google-dataproc/)
