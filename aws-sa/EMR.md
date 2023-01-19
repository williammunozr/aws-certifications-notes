# Amazon EMR

## What is Amazon EMR?

Managed cluster platform that simplifies running big data frameworks.

- `Master Node`: A node that manages the cluster by running software components to coordinate the distribution of data and tasks among other nodes.
- `Core Node`: A node with software components that run tasks and store data in the Hadoop Distributed File System (HDFS) on your cluster. Multi-node clusters have at least one core node.
- `Taks Node`: A node with software components that only runs tasks and does not store data in HDFS task nodes are optional.

### Data Processing Frameworks

- Engine used to process and analyze data
- Different frameworks are available for different kinds of processing needs
- The main processing frameworks available for Amazon EMR are Hadoop MapReduce and Spark

### Cluster Resource Management

- The resource management layer is responsible for managing cluster resources and scheduling the jobs for processing data
- By default, Amazon EMR uses YARN (Yet Another Resource Negotiator)

### Storage

- Hadoop Distributed File System (HDFS) is a distributed, scalable file system for Hadoop
- Using the EMR File System (EMRFS), Amazon EMR extends Hadoop to add the ability to directly access data stored in Amazon S3 as if it were a file system like HDFS
- The local file system refers to a locally connected disk

## Resources

- [Amazon EMR - AWS EMR Tutorial - Full Course in 60 mins](https://www.youtube.com/watch?v=v9nk6mVxJDU)
- [Amazon EMR on EKS](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/emr-eks.html)
