---
title: "2019-11-08-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-11-02 ~ 2019-11-08"
date: 2019-11-02 ~ 2019-11-08
description: "This is the Pulsar community weekly update for 2019-11-02 ~ 2019-11-08, with updates on the sticky consumer for key-shared subscription, producers support producing messages with different schemas, the release of BookKeeper 4.10, and more."
---


## [Pulsar Community Weekly Update] 2019-11-02 ~ 2019-11-08

This is the Pulsar community weekly update for 2019-11-02 ~ 2019-11-08, with updates on the sticky consumer for key-shared subscription, producers support producing messages with different schemas, the release of BookKeeper 4.10, and more.

### Pulsar Development

- [PIP-49][Permissions] The discussion of improvements of permissions continues. The scope of the PIP is proposed to reduce to focus on documenting the permissions for admin API and make the implementation stick to it.

    https://github.com/apache/pulsar/wiki/PIP-49%3A-Permission-levels-and-inheritance
    

- [PIP-43][Schema] PIP-43 is completed. Producers now are able to send messages with different schemas. Many thanks to Yi Tang for this incredible contribution.

    https://github.com/apache/pulsar/wiki/PIP-43%3A-producer-send-message-with-different-schema
    
- [PIP-34] Penghui Li introduced sticky consumers for `key_shared` subscription. This provides the ability for implementing an exactly-once source connector for Flink with auto-scaling.

    https://github.com/apache/pulsar/pull/5388
    
- [Pulsar Manager] Pulsar Manager starts the vote for its first Apache release.

    https://lists.apache.org/thread.html/eb7766661380652fd61ba09c1f6bf198c49b7f45dac9915908a073d1@%3Cdev.pulsar.apache.org%3E
    
- [BookKeeper] Apache BookKeeper has successfully voted its 4.10 release. Pulsar is bumping bookkeeper version to 4.10 in its coming releases.

    https://lists.apache.org/thread.html/b4f1545bd23552e7fe9f9946b73c135e4d49a0717af8a1051913b48e@%3Cdev.bookkeeper.apache.org%3E

### Notable Feature

- [Connectors] Add subscribe position param for consumers of input topics of a sink (Release: 2.4.2, 2.5.0)

    https://github.com/apache/pulsar/pull/5532

- [Client][C++/Python] Increase number of digits in temporary subscription name for readers (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5547

- [Client][C++/Python] Add seek-by-time support for C++ and Python clients (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5542

### Notable Bug Fix

- [Schema] Fix "Trying to subscribe with incompatible schema" (Release: 2.4.2, 2.5.0)

    https://github.com/apache/pulsar/issues/4790
    
    https://github.com/apache/pulsar/pull/5563

- [Schema][Functions] Fix Java function errors using Protobuf schema (Release: 2.4.2, 2.5.0)

    https://github.com/apache/pulsar/pull/5569
    
- [Kubernetes][Prometheus] Fix ZooKeeper kubernetes annotations for prometheus pull metrics from port 8000 (Release: 2.4.2, 2.5.0)

    https://github.com/apache/pulsar/pull/5601

### Event/News

* [Conference] Devoxx was held on November 4-8 in Belgium. Quentin Adam and Steven Le Roux presented this conference and shared Architecture, Concepts, and  Benchmarks of Apache Pulsar. 
    
    https://www.youtube.com/watch?v=De6avNyQUMw
    
* [Conference] 4th Workshop on Real-time & Stream Analytics in Big Data & Stream Data Management is coming on December 9-12 in Los Angeles. Matteo Merli will attend and give a talk about Apache Pulsar.
    
    https://workshop.euranova.eu/bigdata19.html
    
* [Anniversary] Apache BookKeeper celebrated the 5th anniversary this month.

    https://projects.apache.org/committee.html?bookkeeper

### Blog/Article

* Apache Pulsar — One Cluster for the Entire Enterprise Using Multi-Tenancy (by Karthikeyan Palanivelu)

    https://medium.com/capital-one-tech/apache-pulsar-one-cluster-for-the-entire-enterprise-using-multi-tenancy-ac0bd925fbdf
    
* Apache Pulsar: configuring tiered-storage (AWS S3) via HELM (by Thomas Memenga)

    https://www.syscrest.com/2019/11/apache-pulsar-tiered-storage-helm-aws-s3/