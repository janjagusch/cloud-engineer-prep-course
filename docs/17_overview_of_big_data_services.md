# Overview of Big Data Services

## Introduction to Cloud PubSub 1

* Message queue service
* Asynchronous
* Topic: Structure for storing messages
* Subscription: Enables application to read messages from a topic

## Introduction to Cloud PubSub 2

* Create topic
    * Topic id
* Create subscription
    * Subscription id
    * Delivery type (pull, push)
    * Expiration date
    * Ack deadline
    * Message retention duration
* Publish message
* Create a snapshot
    * To save the state of the topic

## Introduction to Cloud Dataproc

* Service that manages Hadoop clusters for us
* Create cluster
    * Cluster mode (number of master and worker nodes)
    * Master machine type
    * Master primary disk size/type
    * Worker machine type (vertical or horizontal scaling)
    * Worker primary disk size/type
    * Number of worker nodes
    * Preemtible worker nodes
* Create jobs
    * Job type (Hadoop, Spark, PySpark, Hive, Pig, etc.)

## Introduction to Cloud Dataflow

* Stream and batch processing framework based on Apache Beam
* Runs jobs written in Java or Python
* ETL
* Temporary files are written in GCS
* Serverless
* DAG
* Lots of templates

## Introduction to Cloud Transfer

* Used for transfering from one bucket to a GCP bucket
* Also for scheduling jobs
* Source could be AWS S3, destination is always GCP
* Extra filters
* Overwrite policy

## Introduction to BigQuery

* Analytics, data warehousing database
* Uses SQL, but not relational database
* Command line `bq`
* Data transfer service

## Quiz

What service would you use to transfer 30TB of data to Cloud Storage from your on premises data center?

> Data Transfer Appliance (not Service)

What service would you use to process an IoT stream of time series data and create summary statistics for each minute of data?

> Cloud Dataflow

What kind of subscription would you create on a Cloud Pub/Sub topic if you want the program processing the messages to control when the message is read?

> Pull subscription

Your manager would like to stop managing a Hadoop cluster after migrating to GCP. What service would you recommend using to replaced a self-managed Hadoop cluster?

> Dataproc