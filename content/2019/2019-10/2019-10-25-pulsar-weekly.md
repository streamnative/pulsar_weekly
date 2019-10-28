---
title: "2019-10-25-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-10-19 ~ 2019-10-25"
date: 2019-10-19 ~ 2019-10-25
description: "This is the weekly community update for 2019-10-19 ~ 2019-10-25, which helps you quickly capture Pulsar's highlights and spot trends over last week, meanwhile strengthen the communication and connection within the Pulsar family."
---


## [Community Weekly Update] 2019-10-19 ~ 2019-10-25 

This is the weekly community update for 2019-10-19 ~ 2019-10-25, which helps you quickly capture Pulsar's highlights and spot trends over last week, meanwhile strengthen the communication and connection within the Pulsar family.

### Pulsar Development

* [CI] ASF Jenkins is back to 'normal' after reverting 'Add default loader for latest pyyaml (#4974)' [1] in #5432 [2]. The problem was from the usage of pyyaml in python 2.7 causing function workers failing to start in integration tests. The committers started merging the pull requests.

    [1] https://github.com/apache/pulsar/pull/4974
    
    [2] https://github.com/apache/pulsar/pull/5432
    
* [PIP-43] The main logic for supporting producers to send message with different schemas was merged. With this change, Pulsar provides the capability of supporting event sourcing applications with different schemas. Kudos to Yi Tang!

    https://github.com/apache/pulsar/pull/5443
    
* [Functions] Jerry Peng started the effort on refactoring functions runtime to make it pluggale. It will make the future development of adding a new runtime easier and more smoothly.

    https://github.com/apache/pulsar/pull/5463
    
* [PIP-45] The second pull request for pluggable metadata interface is out to change the implementation of ManagedLedger to use MetadataStorre interface.

    https://github.com/apache/pulsar/pull/5358
    
* [Key-Shared] Penghui kicked off the implementation of supporting sticky consumers in key_shared subscription. This provides a capability for consuming sub-streams from a given topic (partition) in order. It can be used in Flink integration for supporting flexiblle scaling up-and-down.

    https://github.com/apache/pulsar/pull/5388
    
* [Transaction] The development of TC continues with adding topic ownership listener for bootstraping coordinator when a coordination topic is owned.

    https://github.com/apache/pulsar/pull/5457

### Notable Features

* [Client][Java] Add support for partitioned topic consumer seek by time. (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5435
    
* [Functions] Make Function authentication provider pluggable. (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5404
    
* [Client][Java] Support set read-position based on timestamp. (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5075
    
### Notable Bug Fix

* [Client][CGo] Return message ID for produced messages. (Fixed, Release: 2.5.0)

    https://github.com/apache/pulsar/pull/4811

* [Broker] Fix potential deadlock that can occur in addConsumer. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5371
    
* [Client][Java] Avoid leak on publish failure on batch message. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5442
    
* [Broker] Fix: race condition: failed to read-more entries on dispatcher. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5391
    
* [Client][Java] Fix message corruption on OOM for batch messages. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5443

### Ecosystem

* Pulsar.Client 0.7.0 was released with TLS and token authentication support.

    https://www.nuget.org/packages/Pulsar.Client/
    
* More Pulsar tools, integrations, and resources can also be found at https://github.com/streamnative/awesome-pulsar.

### Event/News

* Apache Pulsar gets more attention by giants like Splunk. On Oct 21, Splunk announced to acquire Streamlio to accelerate efforts in real-time stream processing and containerized multi-tenant cloud platform applications. Streamlio is powered by Apache Pulsar, specializing in designing and operating streaming data solutions at scale in demanding enterprise environments. 

    https://www.splunk.com/blog/2019/10/21/splunk-to-expand-streaming-expertise-announces-intent-to-acquire-streamlio-open-source-distributed-messaging-leader.html

* Paris Data Engineers (meetup)

    Paris Data Engineers was held on Oct 22 in France. Quentin Adam talked about how CleverCloud is using Pulsar for scalable logs processing.
    
    https://www.meetup.com/fr-FR/Paris-Data-Engineers/events/264819837/
    
    
### Blog/Article

* Powering Tencent Billing Platform with Apache Pulsar (by Dezhi Liu)

    https://streamnative.io/blog/tech/2019-10-22-powering-tencent-billing-platform-with-apache-pulsar/

* How to use Apache Pulsar Manager with HerdDB (by Enrico Olivelli)

    https://medium.com/streamnative/how-to-use-apache-pulsar-manager-with-herddb-dd265c955ca4

* Why Nutanix Beam went ahead with Apache Pulsar instead of Apache Kafka? (by Yuvaraj Loganathan)

    https://medium.com/@yuvarajl/why-nutanix-beam-went-ahead-with-apache-pulsar-instead-of-apache-kafka-1415f592dbbb
    
* Basic Pulsar producer and consumer (by Thomas Memenga)

    https://www.syscrest.com/2019/10/basic-pulsar-producer-and-consumer-json-helm-kubernetes/
    
