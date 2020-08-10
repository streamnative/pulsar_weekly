---
title: "2020-08-07-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-08-01 ~ 2020-08-07"
date: 2020-08-01 ~ 2020-08-07
description: "This is the Pulsar community weekly update for 2020-08-01 ~ 2020-08-07, with updates on Pulsar clients, Functions, broker, SQL, schema, proxy, and so on."
id: "2020-08-07-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-08-01 ~ 2020-08-07

This is the Pulsar community weekly update for 2020-08-01 ~ 2020-08-07, with updates on Pulsar clients, Functions, broker, SQL, schema, proxy, and so on.

### Notable Feature

- [Pulsar Admin] Support configuring request timeout.

    https://github.com/apache/pulsar/pull/7698
    
- [Java Client] Perform producer compression from IO threads.

    https://github.com/apache/pulsar/pull/7733
    
- [Function] Support specifying producer configuration for functions and sources.

    https://github.com/apache/pulsar/pull/7721
    
- [Topic policy] Support setting message TTL on topic level.

    https://github.com/apache/pulsar/pull/7738

### Notable Bug Fix

- [Broker] Close the previous reader of the health check topic.
    
    https://github.com/apache/pulsar/pull/7724
    
- [Broker] Fix the nondurable consumer that cannot specify the initial position.

    https://github.com/apache/pulsar/pull/7702
    
- [Function] Fix various issues with batch source.

    https://github.com/apache/pulsar/pull/7716
    
- [Broker] Replay delayed messages in order.

    https://github.com/apache/pulsar/pull/7731
    
- [Broker] Avoid ConcurrentModificationException of LocalBrokerData.

    https://github.com/apache/pulsar/pull/7729
    
- [Schema] Fix the issue of getting schemaName by partitioned topic name.

    https://github.com/apache/pulsar/pull/7708
    
- [Pulsar SQL] Make Pulsar SQL get correct offload configurations.

    https://github.com/apache/pulsar/pull/7708
    
- [Pulsar Proxy] Handle NPE while updating proxy stats.

    https://github.com/apache/pulsar/pull/7766
    
- [Broker] Fix the bug that the producer for geo-replication is not closed when topic is unloaded.

    https://github.com/apache/pulsar/pull/7735
    
- [Proxy] Fix deadlock in Pulsar proxy.

    https://github.com/apache/pulsar/pull/7690
    
- [Broker] Make resetting cursor in REST API asynchronous.

    https://github.com/apache/pulsar/pull/7744
    
- [Broker] Ensure to return Error 404 when deleting a partitioned-topic on a non existing namespace.

    https://github.com/apache/pulsar/pull/7777

### Event / News
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 018: From Single-AZ to Multi-AZ and Geo-replication
  
        - https://www.youtube.com/watch?v=Vc_a2ppRzlI

- [Upcoming event]

  - 08/25: StreamNative Webinar - "Managing Real-Time Data Teams" by Jesse Anderson

    Registration link: https://us02web.zoom.us/webinar/register/6715970153506/WN_fEFcuXVFRWaZxa2pJtP3nQ

### Blog / Article

- Global and local Apache ZooKeeper in Apache Pulsar - part 2 - Bartosz Konieczny 

    - https://streamnative.io/whitepaper/pulsar-vs-kafka
