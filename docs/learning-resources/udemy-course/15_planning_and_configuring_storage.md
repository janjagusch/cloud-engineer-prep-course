# Planning and Configuring Storage

## Types of Storage Systems

## Cloud Storage Buckets and Types of Object Storage

## Versioning and Object Lifecycle Management

## Cloud SQL for Regional Regional Data Storage

## Cloud Spanner for Global Regional Data Storage

* Managed relational database
* Horizontally scalable global database
* Strong consistency within your data and users around the world
* Spanner instance != VM instance
* Spanner instance == Set of VM instances that run the database
* Global multi-region
* First create instance, then create database
* Running spanner can get rather expensive

## Cloud Datastore

* Cloud Datastore: No SQL database
* Two modes to run:
    * Native mode (Firestore API)
    * Datastore mode (Datastore API on top of firestore)
* Serverless
* One database per project

## Cloud Datastore 2

* Create entity
    * Namespace
    * Kind
    * Key-identifier
    * Properties
    * Values
* Index allows us to lookup entities by that value
* Composite index: Index by two or more properties

## Cloud Bigtable

* Managed, NoSQL database
* Wide-column (sparse)
* Low latency, high availability (good for IoT)
* Designed for analytics
* Managed, but not serverless
* Expensive service
* Can specify more than one cluster in a service
    * Nodes store metadata (for lookups, e.g.)
* Storage system: Collusus (also used by Cloud Storage)
* You can create a replicated cluster in a different zone

## Quiz

* What two services provide managed relational databases?

    > Cloud SQL and Cloud Spanner

* What two services provide managed NoSQL databases?

    > Datastore and Bigtable

* You want to have files automatically moved to Nearline storage from a regional storage bucket after the files are 60 days old. How can this be done with the least effort on the part of a storage administrator?

    > Add a lifecycle management rule

* You have a large number of archive files that you will need to store for several years. You are not likely to retrieve any of the files over the 5 years that you have to retain them. What is the most cost-effect storage type to use for this use case?

    > Coldline storage
