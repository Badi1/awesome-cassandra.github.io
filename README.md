# Awesome Cassandra [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
 
## Manage massive amounts of data, fast, without losing sleep

<img src="https://raw.githubusercontent.com/awesome-cassandra/awesome-cassandra.github.io/master/pics/logo-cassandra.png" 
     height="120px" />

The Apache Cassandra database is the right choice when you need scalability and high availability without compromising performance. Linear scalability and proven fault-tolerance on commodity hardware or cloud infrastructure make it the perfect platform for mission-critical data. Cassandra's support for replicating across multiple datacenters is best-in-class, providing lower latency for your users and the peace of mind of knowing that you can survive regional outages.

This is a curated list of awesome [Apache Cassandra](http://cassandra.apache.org/) packages and resources. This list has been initiated and maintained by Rahul Singh of [Anant](http://anant.us). 

This powers the *Resources* section of [Cassandra.Link](https://cassandra.link), a rich collection of blog feeds, and curated links as a searchable knowledge base. 

## Contents

- [General](#general) 

<!-- TODO: list out concept subject titles here and link -->
- [Packages](#packages)
  - [Libraries](#libraries)  Programming Language Specific Libs for Cassandra.
  - [Tools](#tools) Applications / Tools that work with Cassandra.
  - [Projects](#projects) Other projects that use Cassandra.
  - [Queues / Schedulers](#queues--schedulers) 
  - [Logging](#logging)
  - [Open Source Applications](#open-source-applications)
  
- [Resources](#resources) 
  - [Documentation](#documentation) Official / unofficial documentation. 
  - [Books](#books) Popular books about Cassandra.
  - [Courses](#courses) Step by step tutorials on Cassandra.
  - [Communities](#communities) Sites ( not blogs ) on Cassandra.
  - [Blogs](#blogs) from Cassandra experts.
  - [Videos](#videos) Videos on Cassandra.
  - [Slides](#slides) Slides on Cassandra / related technologies.

## General

### Cassandra 
- [Apache Cassandra](http://cassandra.apache.org/) - Manage massive amounts of data, fast, without losing sleep.

### Cassandra History
- [IDG: 10 Years of Apache Cassandra](https://www.idgconnect.com/abstract/30973/apache-cassandra)
- [ZDNet: Apache Cassandra Turns 10](https://www.zdnet.com/article/apache-cassandra-turns-10/)

### Cassandra Use Cases 
- [Datastax Academy: Brief Introduction to Apache Cassandra](https://academy.datastax.com/resources/brief-introduction-apache-cassandra)
- [Kaa application based on Raspberry Pi and DHT11 sensor](https://github.com/pyroalf/kaa-cassandra-sample) - Cassandra IoT usecase with Raspberry Pi and a DHT11 Sensor.
- [Simple Node.js Express 4 Cassandra Application](https://github.com/bradtraversy/mysubscribers) - MySubscribers is a very simple application (Start of an application) which allows you to create, read, update and delete users/subscribers. This application was only created to aid the YouTube course.
- [An Odyssey of Cassandra](http://hadoopmag.com/an-odyssey-of-cassandra/) - This is an old article republished but talks about transitioning from SQL to NoSQL with Cassandra.

### Cassandra Distributions
- [Datastax Enterrpise](https://www.datastax.com/) - Most widely used commercial distribution of Apache Cassandra, integrated with Apache Spark (for SparkSQL, analytics), Apache Solr (for secondary index), Apache TinkerPop based Graph stored in Cassandra, and OpsCenter.
- [DDACS](https://www.datastax.com/products/datastax-distribution-of-apache-cassandra) - Datastax Distribution of Apache Cassandra, a production ready distribution with a bulk loader supported by Datastax. 
- [Elassandra](http://www.elassandra.io/) - Elassandra = Elasticsearch as a Cassandra secondary index.
- [ScyllaDB](https://github.com/scylladb/scylla) - NoSQL data store using the seastar framework, compatible with Apache Cassandra.
- [YugaByte Database](https://github.com/YugaByte/yugabyte-db) - YugaByteDB is a transactional, high-performance database for building distributed cloud services. It supports Cassandra-compatible and Redis-compatible APIs, with PostgreSQL in Beta.
- [Microsoft Azure Cosmos DB: Apache Cassandra API](https://docs.microsoft.com/en-us/azure/cosmos-db/cassandra-introduction) - Azure Cosmos DB provides the Cassandra API (preview) for applications that are written for Apache Cassandra that need premium capabilities.

### Using Cassandra

<!-- - TODO:: cassandra installation tutorials in local, docker, cloud (do, aws, azure, gcp)) -->
<!-- - TODO:: compiling cassandra -->
<!-- - TODO:: running cassandra -->
<!-- - TODO:: using cql -->
<!-- - TODO:: using zeppelin with cassandra -->
<!-- - TODO:: getting data in / out of cassandra -->
<!-- - TODO:: using spark with cassandra -->

- [Installing the Cassandra / Spark OSS Stack](https://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html)
- [Install Cassandra and Spark](http://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html) - Quick user guide for integration with Cassandra and Spark.
- [The Cassandra Query Language](http://cassandra.apache.org/doc/latest/cql/)
- [tghe LIMIT Clause in Apache Cassandra might not work as you think](http://thelastpickle.com/blog/2017/03/07/The-limit-clause-in-cassandra-might-not-work-as-you-think.html)
- [Building a Performant API using Go and Cassandra](https://getstream.io/blog/building-a-performant-api-using-go-and-cassandra/)
- [Cassandra Data Copy Tool](https://github.com/wildengineer/cassandra-data-copy-tool) - Java tool to copy data from one cassandra table to another.
- [Spring Data Cassandra Examples](https://github.com/jxblum/spring-data-cassandra-examples) - Examples for the Spring Data Cassandra Project.
- [Introduction to Spark & Cassandra](http://rustyrazorblade.com/post/2015/2015-01-02-intro-to-spark-and-cassandra/)
- [From Cassandra to S3, with Spark](https://objectpartners.com/2016/11/30/from-cassandra-to-s3-with-spark/)
- [Import CSV files with spark](https://github.com/markthebault/importCSVSparkCassandra) - How to import a file from S3 into cassandra using Spark.
- [Using Apache Cassandra — A few things before you start](https://hackernoon.com/using-apache-cassandra-a-few-things-before-you-start-ac599926e4b8) - Great advice to read before diving deep into Cassandra. 
- [Top 5 reasons to use the Apache Cassandra Database](https://towardsdatascience.com/top-5-reasons-to-use-the-apache-cassandra-database-d541c6448557) - Few good reasons why you'd want to consider Apache Cassandra. 
- [Cloud DevOps with Cassandra](http://cloudurable.com/blog/aws-ansible-packer-ssh-for-devops/index.html) - Using Packer, Ansible/SSH and AWS command line tools to create and DBA manage EC2 Cassandra instances in AWS.
- [How to install Cassandra 2 on CentOS 7 / RHEL 7](https://sharadchhetri.com/2015/04/25/how-to-install-cassandra-2-on-centos-7-rhel-7/) - A guide on hwo to install Cassandra on the popular linux distributions RedHat and CentOS.

<!-- - TODO:: sql v. cql-->
<!-- - TODO:: query driven methodology -->
<!-- - TODO:: schema designs / examples-->
<!-- - TODO:: data modeling problems -->

### Cassandra from Relational
- [RDBMS to NoSQL](http://www.datastax.com/relational-database-to-nosql) - Your roadmap to understanding whether NoSQL is right for you.
- [MySQL to C*](http://planetcassandra.org/mysql-to-cassandra-migration/) - MySQL to Cassandra migration guide.
- [Real-Time Replication from MySQL to Cassandra](https://mcbguru.blog/2014/02/27/real-time-replication-from-mysql-to-cassandra/)
- [Cassandra Schemas for Beginners (like me)](https://medium.com/@jochasinga/cassandra-schemas-for-beginners-like-me-9714cee9236a) - Great article for new developers to Cassandra.
- [Cassandra and Relational database schema comparison – Query vs relationship modeling](https://blog.rdx.com/cassandra-and-relational-database-schema-comparison-query-vs-relationship-modeling/) 
- [Cassandra Query Language: CQL vs SQL](https://medium.com/@alexbmeng/cassandra-query-language-cql-vs-sql-7f6ed7706b4c) 

### Cassandra Data Modeling
- [Basic Rules Of Cassandra Data Modeling](http://www.datastax.com/dev/blog/basic-rules-of-cassandra-data-modeling) - Picking the right data model is the hardest part of using Cassandra. If you have a relational background, CQL will look familiar, but the way you use it can be very different.
- [Cassandra Query Language : CQL vs. SQL](https://medium.com/@alexbmeng/cassandra-query-language-cql-vs-sql-7f6ed7706b4c)
- [CQL: This is not the SQL you are Looking For](https://www.slideshare.net/aploetz/cql-this-is-not-the-sql-you-are-loooking-for)
- [A Deep Look at the CQL Where Clause](https://www.datastax.com/dev/blog/a-deep-look-to-the-cql-where-clause)
- [killrvideo-sample-schema](https://github.com/pmcfadin/killrvideo-sample-schema) - Sample Cassandra CQL Schema for a YouTube clone.
- [Spring Data Cassandra Examples](https://github.com/jxblum/spring-data-cassandra-examples/blob/master/src/main/resources/cassandra-example-schema.cql)
- [Common Problems in Cassandra Data Models](https://blog.anant.us/common-problems-cassandra-data-models/) - Presentation and Article on wide partions, tombstones, and data skew.
- [Casandra Time Series Data Modeling for Massive Scale](http://thelastpickle.com/blog/2017/08/02/time-series-data-modeling-massive-scale.html)
- [Cassandra Data Modeling Notes](https://miguelperez.xyz/blog/2017/2/13/cassandra-data-modeling-notes) - Simple notes on how to estimate the size of your cluster. 
- [Scalar DB](https://github.com/scalar-labs/scalardb) - Transaction library for Cassandra.


<!-- - TODO: - Data Centers and Racks -->
<!-- - TODO: - Gossip and Failure Detection -->
<!-- - TODO: - Snitches -->
<!-- - TODO: - Rings and Tokens -->
<!-- - TODO: - Virtual Nodes -->
<!-- - TODO: - Partitioners -->
<!-- - TODO: - Replication Strategies -->
<!-- - TODO: - Consistency Levels -->
<!-- - TODO: - Queries and Coordinator Nodes -->
<!-- - TODO: - Memtables, SSTables, and Commit Logs -->
<!-- - TODO: - Caching -->
<!-- - TODO: - Hinted Handoff -->
<!-- - TODO: - Lightweight Transactions and Paxos -->
<!-- - TODO: - Tombstones -->
<!-- - TODO: - Bloom Filters -->
<!-- - TODO: - Compaction -->
<!-- - TODO: - Anti-Entropy, Repair, and Merkle Trees -->
<!-- - TODO: - Staged Event-Driven Architecture (SEDA) -->
<!-- - TODO: - Managers and Services -->
<!-- - TODO: - System Keyspaces -->


### Cassandra Architecture
- [The Gossip Protocol - Inside Apache Cassandra.](https://www.linkedin.com/pulse/gossip-protocol-inside-apache-cassandra-soham-saha) - Good visual explanation of how Cassandra keeps consistent. 
- [Introduction To The Apache Cassandra 3.x Storage Engine](http://thelastpickle.com/blog/2016/03/04/introductiont-to-the-apache-cassandra-3-storage-engine.html) - The 3.x storage engine makes it easier for Cassandra to get bytes off disk.
- [Dropping columns in Apache Cassandra 3.0](http://thelastpickle.com/blog/2016/02/18/dropping-columns.html)
- [Hinted Handoff and GC Grace Demystified](http://thelastpickle.com/blog/2018/03/21/hinted-handoff-gc-grace-demystified.html) - Tuning the balance between GC Grace and Hinted Handoff.
- [Deletes an Tombstones](http://thelastpickle.com/blog/2011/05/15/Deletes-and-Tombstones.html) - Explains how deletes create tombstones in Cassandra and what they are. 
- [About Deletes and Tombstones in Cassandra](http://thelastpickle.com/blog/2016/07/27/about-deletes-and-tombstones.html) - Deleting distributed and replicated data from a system such as Apache Cassandra is far trickier than in a relational database.
- [Null bindings on prepared statements and undesired tombstone creation](http://thelastpickle.com/blog/2016/09/15/Null-bindings-on-prepared-statements-and-undesired-tombstone-creation.html) - Good follow up to the last article on Tombstones.
- [Undetecetable tombstones in Apache Cassandra](http://thelastpickle.com/blog/2018/07/05/undetectable-tombstones-in-apache-cassandra.html) - Indepth analysis of cell and range tombstones. 
- [Common Problems with Cassandra Tombstones](https://opencredo.com/cassandra-tombstones-common-issues/) - "Large Number of Tombstones Causes Latency and Heap Pressure".
- [Curious Case of Tombstones](https://medium.com/cassandra-tombstones-clearing-use-case/the-curios-case-of-tombstones-d897f681a378) -  How someone dealt with tombstone issues and reclaimed space in their cluster.
- [Understanding the Nuance of Compaction in Apache Cassandra](http://thelastpickle.com/blog/2017/03/16/compaction-nuance.html) - Overview of how Cassandra manages data on disk.
- [Guide to Cassandra Thread Pools](https://blog.pythian.com/guide-to-cassandra-thread-pools/) - This guide provides a description of the different thread pools and how to monitor them. Includes what to alert on, common issues and solutions. Old but very useful reference. 
- [Cassandra Architecture and Operations](https://miguelperez.xyz/blog/2017/2/13/cassandra-architecture-and-operation) - A high level overview in one page of how Cassandra works. 

### Cassandra Monitoring
- [Resources for Monitoring Datastax, Cassandra, Spark, & Solr Performance](https://blog.anant.us/resources-for-monitoring-datastax-cassandra-spark-solr-performance/)
- [How to Monitor Cassandra](https://www.datadoghq.com/blog/how-to-monitor-cassandra-performance-metrics/) - A guide to help you monitor Cassandra performance and work metrics regardles of which monitoring tool you choose to use.
- [Cassandra metrics and their use in Grafana](https://medium.com/@mlowicki/cassandra-metrics-and-their-use-in-grafana-1f0dc33f9cca)
- [Monitoring Cassandra with Prometheus](https://www.robustperception.io/monitoring-cassandra-with-prometheus)
- [Monitoring Cassandra With Grafana And Influx DB](https://blog.pythian.com/monitoring-cassandra-grafana-influx-db/)
- [Cassandra Monitoring - Introduction (1/2)](https://softwaremill.com/cassandra-monitoring-part-1/)
- [Cassandra Monitoring - Graphite/InfluxDB & Grafana on Docker (1/2)](https://softwaremill.com/cassandra-monitoring-part-2/)
- [Monitoring Cassandra using Intel Snap and Grafana](http://thelastpickle.com/blog/2017/04/13/monitoring-cassandra-using-intel-snap.html) - This blog post describes how to monitor Apache Cassandra using the Intel Snap open source telemetry framework.

<!-- - TODO:: Health Check -->
<!-- - TODO:: Basic Maintenance -->
<!-- - TODO:: Adding Nodes -->
<!-- - TODO:: Handling Node Failure -->
<!-- - TODO:: Upgrading Cassandra -->
<!-- - TODO:: Backup and Recovery -->
<!-- - TODO:: SSTable Utilities -->
<!-- - TODO:: Maintenance Tools  -->
<!--  - OpsCenter  -->
<!--  - Reaper  -->
<!--  - TableAnalyzer  -->

### Cassandra Maintenance
- [Running commands cluster-wide without any management tool](http://thelastpickle.com/blog/2016/03/21/running-commands-cluster-wide.html) - Some tips and tricks to do basic Cluster operations without tools like Chef, Ansible, or Salt.
- [Limiting Nodetool Parallel Threads](http://thelastpickle.com/blog/2017/08/14/limiting-nodetool-parallel-threads.html) - Little known tool to do nodetool operations with less resources.
- [Bootstrapping Cassandra Nodes](http://thelastpickle.com/blog/2017/05/23/auto-bootstrapping-part1.html) - Indepth article on how to add nodes to a running Cassandra cluster.
- [Node Replacement without Bootstrapping](http://thelastpickle.com/blog/2018/02/21/replace-node-without-bootstrapping.html) - How to avoid the long bootstrapping process.
- [Cassandra Backup and Restore - Backup in AWS using EBS Volumes](http://thelastpickle.com/blog/2018/04/03/cassandra-backup-and-restore-aws-ebs.html) - Indepth article about Backup and recovery in AWS.
- [Backup Strategies for Cassandra](https://blog.pythian.com/backup-strategies-cassandra/) - Good comparison of different backup and restoration strategies for Cassandra. 
- [Cassandra backup util](https://github.com/instaclustr/cassandra-backup) - https://GitHub.com/instaclustr/cassandra-backup
- [sstable tools](https://github.com/tolbertam/sstable-tools) - A toolkit for parsing, creating and doing other fun stuff with Cassandra 3.x SSTables.
- [cassandra-sstable-tools](https://github.com/instaclustr/cassandra-sstable-tools) - Tools for working with sstables.
- [Cassy](https://github.com/scalar-labs/cassy) - A simple and integrated backup tool for Apache Cassandra. 

<!-- - TODO:: Managing Performance -->
<!-- - TODO:: Caching -->
<!-- - TODO:: Memtables -->
<!-- - TODO:: Commit Logs -->
<!-- - TODO:: SSTables -->
<!-- - TODO:: Hinted Handoff -->
<!-- - TODO:: Compaction -->
<!-- - TODO:: Concurrency and Threading -->
<!-- - TODO:: Networking and Timeouts -->
<!-- - TODO:: JVM Settings -->
<!-- - TODO:: Using cassandra-stress -->
<!-- - TODO:: Using Gatling -->


### Cassandra Performance Tuning
- [Jon Haddad: Cassandra Summit Recap - Diagnosing Problems in Production](http://rustyrazorblade.com/2014/09/cassandra-summit-recap-diagnosing-problems-in-production/)
- [A Deeper Dive - Diagnosing DSE Performance Issues with Ttop and Multidump](https://academy.datastax.com/support-blog/deeper-dive-diagnosing-dse-performance-issues-ttop-and-multidump) - A good review of how to look deeper into Cassandra threads. 
- [Ryan Svihla's Cassandra 2.0 checklist](https://medium.com/@foundev/my-cassandra-diagnostics-checklist-brain-dump-599a2b95b118)
- [Amy's Cassandra 2.1 tuning guide](https://tobert.github.io/pages/als-cassandra-21-tuning-guide.html)
- [Secret HotSpot option improving GC pauses on large heaps](http://blog.ragozin.info/2012/03/secret-hotspot-option-improving-gc.html)
- [DSE 5.1: Tuning Java Resource](https://docs.datastax.com/en/dse/5.1/dse-admin/datastax_enterprise/operations/opsTuneJVM.html)
- [Analyzing Cassandra Performance with Flame Graphs](http://thelastpickle.com/blog/2018/01/16/cassandra-flame-graphs.html) - Visually examining Cassandra performance visually using Flamegraphs. 
- [Garbage Collection Tuning for Cassandra](http://thelastpickle.com/blog/2018/04/11/gc-tuning.html) - Optimizing garbage collection for better performance.
- [Cassandra Node Diagnostics Tools](https://github.com/smartcat-labs/cassandra-diagnostics) - Monitoring and audit power kit for Apache Cassandra.
- [TWCS part 1 - how does it work and when should you use it?](http://thelastpickle.com/blog/2016/12/08/TWCS-part1.html) - Best suited for time series data that expires, Time Window Compaction Strategy comes with some caveats.
- [Performing User Defined Compactions in Apache Cassandra](http://thelastpickle.com/blog/2016/10/18/user-defined-compaction.html) - This is a process by which we tell Cassandra to create a compaction task for one or more tables explicitly. 
- [Graphing cassandra-stress](http://thelastpickle.com/blog/2015/10/23/cassandra-stress-and-graphs.html) - Benchmarking schemas and configuration changes using the cassandra-stress tool, before pushing such changes out to production is one of the things every Cassandra developer should know and regularly practice.
- [Modeling real life workloads with cassandra-stress is hard](http://thelastpickle.com/blog/2017/02/08/Modeling-real-life-workloads-with-cassandra-stress.html)  
- [Gatling DSE Stress](https://github.com/datastax/gatling-dse-stress)
- [Gatling DSE Plugin for Gatling Load injector](https://github.com/datastax/gatling-dse-plugin) - This project is a plugin for the Gatling load injector. It adds CQL support in Gatling for Datastax Enterprise. It allows for benchmarking Datastax Enterprise features, including DSE Graph Fluent API.
- [Gatling DSE Stress Simulation Catalog](https://github.com/datastax/gatling-dse-simcatalog) - The goal of the repo is to provide a sample of the Gatling DSE Stress Framework's usage. Feel free to submit a pull request with example simulations.


<!-- - TODO:: Authentication and Authorization -->
<!-- - TODO:: Encryption -->
<!-- - TODO:: JMX Security -->
<!-- - TODO:: Disk -->
<!-- - TODO:: System -->
<!-- - TODO:: Network -->


### Cassandra Security
- [Securing Apache Cassandra with Application Level Encryption](https://www.instaclustr.com/securing-apache-cassandra-with-application-level-encryption/) - Discusses how to do application level data encryption to properly manage secure information in Cassandra. 
- [Hardening Cassandra Step by Step: Part 1](http://thelastpickle.com/blog/2015/09/30/hardening-cassandra-step-by-step-part-1-server-to-server.html) - Inter-Node Encryption (And a Gentle Intro to Certificates).
- [LDAP Authenticator for Apache Cassandra](https://github.com/instaclustr/cassandra-ldap) - This is a pluggable authentication implementation for Apache Cassandra, providing a way to authenticate and create users based on a configured LDAP server. 
- [Encrypting EC2 ephemeral volumes with LUKS and AWS KMS](https://www.whaletech.co/2016/04/07/encryption-ephemeral-volumes-with-kms.html) - The example used here is Cassandra data stored on ephemeral disks.


<!-- - TODO:: Planning a Cluster Deployment -->
<!-- - TODO:: Container Deployment -->
<!-- - TODO:: Container Orchestration -->
<!-- - TODO:: Cloud Deployment -->
<!-- - TODO:: Cloud Automations -->

### Deploying Cassandra
- [Setting Up Cassandra Cluster Through Ansible](https://blog.knoldus.com/setting-up-cassandra-cluster-through-ansible/) - A guide detailing how to set up a Cassandra cluster with automation using Ansible.
- [Docker Meet Cassandra. Cassandra Meet Docker](http://thelastpickle.com/blog/2018/01/23/docker-meet-cassandra.html) - Article reviewing how to setup a complete Cassandra application with monitoring on Docker.
- [Example code from the Docker Meet Cassandra Article](https://github.com/thelastpickle/docker-cassandra-bootstrap)
- [Docker-Cassandra](https://github.com/nicolasff/docker-cassandra) - A set of scripts and config files to run a Cassandra cluster from Docker.
- [Cassandra & Zeppelin Notebook on Docker](https://github.com/academyofdata/cassandra-zeppelin) - Docker-Compose script for Cassandra + Zeppelin setup.
- [Packer: Cassandra Image](https://github.com/cloudurable/cassandra-image) - Cassandra Image using Packer for Docker and EC2 AMI. Covers managing EC2 Cassandra clusters with Ansible.
- [Cassandra Docker](https://github.com/instaclustr/cassandra-docker) - This is the Instaclustr public docker image for Apache Cassandra. It contains docker images for Cassandra 3.0 and 3.11.1.
- [Cassandra / Elassandra Docker](https://github.com/zegelin/cassandra-docker) - Apache Cassandra and Elassandra docker images.
- [Instaclustr - Kubernetes Operator for Cassandra](https://github.com/instaclustr/cassandra-operator) - The Cassandra operator manages Cassandra clusters deployed to Kubernetes and automates tasks related to operating an Cassandra cluster.
- [Sky UK - Cassandra Kubernetes Operator](https://github.com/sky-uk/cassandra-operator) - Kubernetes operator that manages Cassandra clusters inside Kubernetes. Well designed and organized. 
- [CassKop - Cassandra operator for Kubernetes](https://github.com/Orange-OpenSource/cassandra-k8s-operator) - This Kubernetes operator automates the Cassandra operations such as deploying a new rack aware cluster, adding/removing nodes, configuring the C and JVM parameters, upgrading JVM and C versions. Written in Go.
- [Running Cassandra on DC/OS (Mesos)](http://thelastpickle.com/blog/2016/05/07/dcos.html) -  This blog will show how to setup DC/OS in the Amazon cloud, how to install Apache Cassandra on a DC/OS cluster, and finally new ways to interact with and Apache Cassandra after it is installed.
- [How To Setup A Highly Available Multi-AZ Cassandra Cluster On AWS EC2](http://highscalability.com/blog/2016/8/1/how-to-setup-a-highly-available-multi-az-cassandra-cluster-o.html)
- [CloudFormation Cassandra AWS](https://github.com/LoyaltyOne/cassandra-aws) - A cassandra cluster for development using Cloud Formation.
- [tlp-cluster, a tool for launching Cassandra clusters in AWS](https://github.com/thelastpickle/tlp-cluster) - A provisioning tool for Apache Cassandra designed for developers looking to both benchmark and test the correctness of Apache Cassandra. It assists with builds and starting instances on AWS.

### Integrating with Cassandra

- [Building a Streaming Data Hub with Elasticsearch, Kafka and Cassandra](http://thenewstack.io/building-streaming-data-hub-elasticsearch-kafka-cassandra/)
- [Docker container for Kafka - Spark streaming - Cassandra](https://github.com/Yannael/kafka-sparkstreaming-cassandra) - This Dockerfile sets up a complete streaming environment for experimenting with Kafka, Spark streaming (PySpark), and Cassandra.
- [sample KafkaSparkCassandra](https://github.com/instaclustr/sample-KafkaSparkCassandra) - Introductory sample scala app using Apache Spark Streaming to accept data from Kafka and write a summary to Cassandra.
- [sample Spark Cassandra with SSL](https://github.com/instaclustr/sample-SparkCassandrawithSSL) - Simple sample job illustrating the use of Spark to execute Apache Spark analytics with Cassandra with SSL connection.

<!-- - TODO:: ESB -->
<!-- - TODO:: Streaming -->
<!-- - TODO:: ETL -->
<!-- - TODO:: CDC -->

#### Spark
- [DataStax Spark Cassandra Connector](https://github.com/datastax/spark-cassandra-connector) - This library lets you expose Cassandra tables as Spark RDDs, write Spark RDDs to Cassandra tables, and execute arbitrary CQL queries in your Spark applications.
- [Stratio Deep (deprecated)](https://github.com/Stratio/stratio-deep) - Deep is a thin integration layer between Apache Spark and several NoSQL datastores. We actually support Apache Cassandra and MongoDB, but in the near future we will add support for sever other datastores.
- [sample Spark Job Server Cassandra](https://github.com/instaclustr/sample-SparkJobserverCassandra) - Simple sample job illustrating the use of Spark Jobserver to execute Apache Spark analytics with Cassandra.
- [fluxcapacitor/pipeline](https://github.com/fluxcapacitor/pipeline) - End-to-End, Real-time, Advanced Analytics Big Data Reference Pipeline using Spark, Spark SQL, Spark ML, GraphX, Spark Streaming, Kafka, NiFi, Cassandra, ElasticSearch, Redis, Tachyon, HDFS, Zeppelin, iPython/Jupyter Notebook, Tableau, Twitter Algebird.


#### Search / Secondary Indexes 
- [Tuning DSE Search](http://www.datastax.com/dev/blog/tuning-dse-search) - Tuning DSE Search – Indexing latency and query latency.
- [Elassandra](http://www.elassandra.io/) - Elassandra = Elasticsearch as a Cassandra secondary index.
- [Cassandra Lucene Index](https://github.com/Stratio/cassandra-lucene-index) - Lucene based secondary indexes for Cassandra.
- OLD - [Solandra](https://github.com/tjake/Solandra) - Solandra is a real-time distributed search engine built on Apache Solr and Apache Cassandra.
- [cassandra-trigger](https://github.com/gradeup/cassandra-trigger) - Cassandra trigger to push realtime updates to elasticsearch.

## Packages


### Libraries
- [express-cassandra](https://github.com/masumsoft/express-cassandra) - Cassandra ORM/ODM/OGM for Node.js with optional support for Elassandra & JanusGraph.
- [DataStax Java Driver](https://github.com/datastax/java-driver) - A Java client driver for Apache Cassandra. 
- [DataStax C++ Driver](https://github.com/datastax/cpp-driver) - A modern, feature-rich, and highly tunable C/C++ client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's native protocol and Cassandra Query Language v3. 
- [DataStax Python Driver](https://github.com/datastax/python-driver) - A modern, feature-rich and highly-tunable Python client library for Apache Cassandra (2.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax Ruby Driver](https://github.com/datastax/ruby-driver) - A Ruby client driver for Apache Cassandra. This driver works exclusively with the Cassandra Query Language version 3 (CQL3) and Cassandra's native protocol.
- [DataStax Node.js Driver](https://github.com/datastax/nodejs-driver) - A modern, feature-rich and highly tunable Node.js client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax C# Driver](https://github.com/datastax/csharp-driver) - A modern, feature-rich and highly tunable C# client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax PHP Driver](https://github.com/datastax/php-driver) - DataStax PHP Driver for Apache Cassandra.
- [Achilles](http://doanduyhai.github.io/Achilles/) - Achilles is an open source Persistence Manager for Apache Cassandra,with the features like Advanced bean mapping (compound primary key, composite partition key, timeUUID...),Native collections and map support,and so.
- [phpcassa](https://github.com/thobbs/phpcassa) - PHP client library for Apache Cassandra.
- [Caffinitas](https://bitbucket.org/snazy/caffinitas/src/develop/) - Caffinitas is an advanced object mapper for Apache Cassandra which has been especially designed to work with Datastax Java Driver 2.1+ against Apache Cassandra 2.1, 2.0 or 1.2.
- [Spring Data for Apache Cassandra](http://projects.spring.io/spring-data-cassandra/) -  Spring Data for Apache Cassandra offers a familiar interface to those who have used other Spring Data modules in the past.
- [gocql](https://github.com/gocql/gocql) - Package gocql implements a fast and robust Cassandra client for the Go programming language.
- [Netflix Astyanax](https://github.com/Netflix/astyanax) - This is an old library. Astyanax was a high level Java client for Apache Cassandra, based on Thrift protocol. Not maintained any more. 
- [Scalar DB](https://github.com/scalar-labs/scalardb) - Transaction library for Cassandra.

### Tools
- [CassandraCAS](https://github.com/Datomic/CassandraCAS) - A compare-and-swap tool for Cassandra created by Datomic.
- [peloton](https://github.com/uber/peloton) - A unified resource scheduler created by Uber. This tool can handle many nodes and clusters through resource management and scalability.
- [ansible-dse](https://github.com/rackerlabs/ansible-dse) - A set of Ansible playbooks that will build a Datastax Enterprise cluster.
- [DbSchema - Cassandra Designer](https://www.dbschema.com/cassandra-designer-tool.html) - DbSchema: Cassandra Diagram Designer & GUI Admin Tool which can do Cassandra amongst other databases. 
- [DBEaver - Free Universal Database Tool](https://dbeaver.io/) - A third party tool for dealing with all sorts of databases including Cassandra. 
- [RazorSQL - Multi DB Manager Tool](https://razorsql.com/) - A multi-db tool for Linux, Mac, and Windows that works with Apache Cassandra. 
- [KDM - The Kashlev Data Modeler](http://kdm.dataview.org/) - An automated big data modeling tool for Apache Cassandra.
- [Cassandra Reaper](http://cassandra-reaper.io/) - Automated repairs for Apache Cassandra. Supports all versions. 
- [cstar perf](https://github.com/datastax/cstar_perf) - Apache Cassandra performance testing platform.
- [Spark Cassandra Stress](https://github.com/datastax/spark-cassandra-stress) - A tool for testing the DataStax Spark Connector against Apache Cassandra or DSE.
- [trireme](https://github.com/o19s/trireme) - Migration tool providing support for Apache Cassandra, DataStax Enterprise Cassandra, & DataStax Enterprise Solr.
- [cqlmigrate](https://github.com/sky-uk/cqlmigrate) -  Cassandra CQL migration tool. cqlmigrate is a library for performing schema migrations on a cassandra cluster.
- [cassandra-migration-tool-java](https://github.com/smartcat-labs/cassandra-migration-tool-java) - Cassandra migration tool for java is a lightweight tool used to execute schema and data migration on Cassandra database. 
- [cassalog](https://github.com/hawkular/cassalog) - Cassalog is a schema change management library and tool for Apache Cassandra that can be used with applications running on the JVM.
- [cdeploy](https://github.com/rackerlabs/cdeploy) - Cdeploy is a simple tool to manage your Cassandra schema migrations in the style of dbdeploy.
- [Web: Cassandra Calculator](https://www.ecyrd.com/cassandracalculator/) - A simple calculator to see how size / replication factor affect the system's consistency.
- [Cassandra-web](http://avalanche123.com/cassandra-web/) - A web interface for Apache Cassandra.
- [CassanddraRestfulAPI](https://github.com/rohitsakala/CassandraRestfulAPI) - CassandraRestfulAPI project exposes the cassandra data tables with the help of Restful API.
- [Netflix: Staash](https://github.com/Netflix/staash) - A language-agnostic as well as storage-agnostic web interface for storing data into persistent storage systems, the metadata layer abstracts a lot of storage details and the pattern automation APIs take care of automating common data access patterns.
- [cql-vim](https://github.com/elubow/cql-vim) - Cassandra CQL Syntax Highlighter for Vim.
- [Presto](https://prestodb.io/) - Distributed SQL Query Engine for Big Data. Presto allows querying data where it lives, including Hive, Cassandra, relational databases or even proprietary data stores. 
- [Sstable Tools](https://github.com/tolbertam/sstable-tools) - A toolkit for parsing, creating and doing other fun stuff with Cassandra 3.x SSTables. 
- [cassandra-exporter](https://github.com/masumsoft/cassandra-exporter) - Simple Tool to Export / Import Cassandra Tables into JSON.
- [Cassandra SStable Tools](https://github.com/instaclustr/cassandra-sstable-tools) - A few different tools combined into one that helps admins get summaries, metadata, partition info, cell info. 
- [Cassandra-Client](https://github.com/Kindrat/cassandra-client) - A simple gui tool for browsing tables and data in Cassandra. 
- [CQL Data Modeler](https://www.sestevez.com/sestevez/CassandraDataModeler/) - A very useful tool to test out a CQL schema and visualize what the partition would like in relationship to the columns and rows. 
- [Cassandra Snapshot Backup](https://github.com/avinash-mishra/cassandra_snapshot_backup) - A quick and easy way to snapshot files in a Cassandra database and back them up using Ansible. 
- [Cassandra Operator](https://github.com/sky-uk/cassandra-operator) - A Kubernetes operator that manages Cassandra clusters inside Kubernetes. Note: This is still in alpha and not recommended for production environments. 
- [Slothsandra](https://github.com/MacKittipat/slothsandra) - An integration for Cassandra with the Slack app, which stores old messages that Slack no longer does itself. 
- [sandraREST](https://github.com/aksakalli/sandraREST) - A Cassandra manager with a web UI for RESTful APIs.
- [Cassandra Leadership](https://github.com/paradoxical-io/cassandra.leadership) - A library to help elect leaders using cassandra. Uses paxos to build a leadership election module.
- [Terraform Cassandra](https://github.com/conrad-mukai/terraform-cassandra) - A terraform module that creates a Cassandra cluster.
- [datadog](https://www.datadoghq.com/blog/monitoring-cassandra-with-datadog/) - A third party tool that allows monitoring and metrics for Cassandra nodes and clusters.
- [tlp-cluster](http://thelastpickle.com/tlp-cluster/) - A provisioning tool for Apache Cassandra designed for developers looking to benchmark and test Apache Cassandra. It assists with builds and starting instances on AWS.
- [Helenos](https://github.com/tomekkup/helenos) - A free web based environment that simplifies a data exploring & schema management with Apache Cassandra database.

### Projects
- [DataStax OpsCenter](http://www.datastax.com/what-we-offer/products-services/datastax-opscenter) - Simplified management for DataStax Enterprise and Cassandra database clusters.
- [Cassandra Cluster Admin](https://github.com/sebgiroux/Cassandra-Cluster-Admin) - Cassandra Cluster Admin is a GUI tool to help people administrate their Apache Cassandra cluster.
- [Cassandra StatD Agent](https://github.com/lookout/cassandra-statsd-agent) - Java Agent for Cassandra integration with StatsD.
- [Cassandra Scripts](https://github.com/bart613/cassandra) - Python based cassandra ops scripts to monitor cfstats. 
- [Cassandra-Tools](https://github.com/CrowdStrike/cassandra-tools) - Python Fabric scripts to help automate the launching and managing of cluster testing on AWS. 
- [Cassandra Opstools](https://github.com/spotify/cassandra-opstools) - Generic scripts to review and monitor cassandra, from Spotify.  
- [CCM: Cassandra Cluster Manager)](https://github.com/pcmanus/ccm) - A script/library to create, launch and remove an Apache Cassandra cluster on localhost.
- [Cassandra Nagios](https://github.com/causes/cassandra-nagios) - Perl Based scripts to get metrics for monitoring using Jolokia.
- [Cassandra Log Tools](https://github.com/erickramirezDSE/cass_log_tools) - Simple scripts for working with Apache Cassandra logs.
- [Cassandra CFStats to CSV Parser](https://github.com/jlacefie/cfstats-csv-parser) - Converts the output of CFStats to CSV. 
- [Netflix-Priam](https://github.com/Netflix/Priam) - Co-Process for backup/recovery, Token Management, and Centralized Configuration management for Cassandra.
- [CStar](https://github.com/spotify/cstar) - Apache Cassandra cluster orchestration tool for the command line.
- [ctop](https://github.com/pixonic/ctop) - This is a very simple console tool for monitoring column families read/write activities at remote cassandra host.

### Queues / Schedulers
- [CMB](https://github.com/Comcast/cmb) - A highly available, horizontally scalable queuing and notification service compatible with AWS SQS and SNS.
- [CassieQ](https://github.com/paradoxical-io/cassieq) - A Distributed queue built off of Cassandra.
- [Cherami](https://eng.uber.com/cherami/) - Distributed, scalable, durable, and highly available message queue system.
- [scheduler](https://github.com/PagerDuty/scheduler) - A Scala library for scheduling arbitrary code to run at an arbitrary time.



### Logging 
- [cassandra-log4j-appender](https://github.com/datastax/cassandra-log4j-appender) - Cassandra appenders for Log4j.

### Open Source Applications 
- [Twissandra](https://github.com/twissandra/twissandra) - Twissandra is an example project, created to learn and demonstrate how to use Cassandra. Running the project will present a website that has similar functionality to Twitter.
- [FiloDB](https://github.com/filodb/FiloDB) - High-performance distributed analytical database + Spark SQL queries + built for streaming.
- [ChronoServer](https://github.com/cyngn/ChronoServer) - A test server for sampling how long it takes mobile & web clients to make various types of requests to a server doing common request patterns. 

## Resources 

### Documentation 
- [Apache Cassandra Documentation](http://cassandra.apache.org/doc/) - Definitive documentation for all published versions. 
- [DataStax Documentation](http://docs.datastax.com/en/landing_page/doc/landing_page/current.html) - Documentation and Drivers from DataStax.

### Books
- [Cassandra: The Definitive Guide, 2nd Edition](http://shop.oreilly.com/product/0636920043041.do)
- [Cassandra High Availability](https://www.packtpub.com/big-data-and-business-intelligence/cassandra-high-availability)

### Courses 
- [DataStax Academy](https://academy.datastax.com/) - Free online courses on Cassandra.

### Communities
- [Apache Cassandra Users Mailing List](http://www.mail-archive.com/user@cassandra.apache.org/)
- [Apache Cassandra Developers Mailing List](http://www.mail-archive.com/dev@cassandra.apache.org/)
- [Apache Cassandra Commits Mailing List](http://www.mail-archive.com/commits@cassandra.apache.org/)
- [Apache Software Foundation Slack](https://s.apache.org/slack-invite) - The #cassandra and #cassandra-dev channels are official slack channels migrating from IRC.
- [Datastax Academy Slack](https://academy.datastax.com/slack)
- [Cassandra Slack](https://cassandra-slack.herokuapp.com/)
- [Stack Overflow: Cassandra](https://stackoverflow.com/questions/tagged/cassandra)
- [Stack Overflow: cql](https://stackoverflow.com/questions/tagged/cql)
- [Stack Overflow: spark-cassandra-connector](https://stackoverflow.com/questions/tagged/spark-cassandra-connector)
- [Quora: Cassandra](https://www.quora.com/topic/Cassandra-database)
- [Meetups: Cassandra](https://www.meetup.com/topics/cassandra/?_cookie-check=mHgLvBy3N6Cke1RU)

### Blogs
- [Datastax](https://www.datastax.com/blog)
- [Datastax Academy](https://academy.datastax.com/developer-blog)
- [Codecentric: Cassandra](https://blog.codecentric.de/en/tag/cassandra/)
- [Pythian: Cassandra](https://blog.pythian.com/technical-track/cassandra-2/)
- [Instaclustr](https://www.instaclustr.com/blog/) 
- [Altheroot:Cassandra](https://blog.alteroot.org/categories/cassandra/index.html)
- [OpenCredo:Cassandra](https://opencredo.com/tag/cassandra/)
- [DOAN DuyHai's Blog: Cassandra](http://www.doanduyhai.com/blog/?cat=57)
- [Amy Tobert](https://tobert.github.io/)
- [Christopher Batey: Cassandra](http://batey.info/cassandra.html)
- [Distributed Bytes:Cassandra](https://distributedbytes.timojo.com/search/label/cassandra)
- [The Netflix Tech Blog](https://medium.com/netflix-techblog)
- [Ryan Svilha](https://lostechies.com/ryansvihla/tags)
- [Anant](https://blog.anant.us/tag/datastax/)

### Videos 
- [Best Practices for Running Cassandra on AWS](https://www.youtube.com/watch?v=IuJldwJLyFM)
- [Monitoring Cassandra: Don't Miss a Thing (Alain Rodriguez, The Last Pickle) | C* Summit 2016](https://www.youtube.com/watch?v=Q9AAR4UQzMk)
- [GumGum: Multi-Region Cassandra in AWS](https://academy.datastax.com/resources/Multi-Region-Cassandra-in-AWS)
- [Tuning the Spark Cassandra Connector](https://www.youtube.com/watch?v=cKIHRD6kUOc&feature=youtu.be) - Great talk by Russell Spitzer maintainer of the Spark Cassandra connector. 

### Slides
- [Cassandra DataTables Using Restful API](https://www.slideshare.net/SimranKedia2/cassandra-datatables-using-restful-api) - A case on how to create a performant API using Python / Flash.
- [HAPI Cassandra](https://github.com/victorcouste/hapi-cassandra) - A simple REST API with hapi Node.js framework on top of a Apache Cassandra database.
- [GumGum: Multi-Region Cassandra in AWS](https://www.slideshare.net/planetcassandra/gumgum-multiregion-cassandra-in-aws)
- [CQL: This is not the SQL you are Looking For](https://www.slideshare.net/aploetz/cql-this-is-not-the-sql-you-are-loooking-for)
- [Hardening cassandra for compliance or paranoia](https://www.slideshare.net/zznate/hardening-cassandra-for-compliance-or-paranoia)
- [Securing Cassandra](https://www.slideshare.net/planetcassandra/securing-cassandra-the-right-way)
- [Tuning the Spark Cassandra Connector](https://www.slideshare.net/DataStax/maximum-overdrive-tuning-the-spark-cassandra-connector-russell-spitzer-datastax-c-summit-2016) - Slides by Russell Spitzer maintainer of the Spark Cassandra connector. 
