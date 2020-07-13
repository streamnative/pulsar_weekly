---
title: "2020-07-10-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-07-04 ~ 2020-07-10"
date: 2020-07-04 ~ 2020-07-10
description: "This is the Pulsar community weekly update for 2020-07-04 ~ 2020-07-10, with updates on Pulsar authentication, connectors, Functions, geo replication, and so on."
id: "2020-07-10-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-07-04 ~ 2020-07-10

This is the Pulsar community weekly update for 2020-07-04 ~ 2020-07-10, with updates on Pulsar authentication, connectors, Functions, geo replication, and so on.

### Notable Feature

- [Broker] Read the usage from `/sys/fs/cgroup/cpu/cpuacct.usage` when using CPU limits on a Docker container.

    https://github.com/apache/pulsar/pull/7475
    
- [C++ Client] Add support for OAuth2 authentication.

    https://github.com/apache/pulsar/pull/7467
    
- [Function] Differentiate authorization between source/sink/function operations.

    https://github.com/apache/pulsar/pull/7466
    
- [Function] Allow function rebalance to run periodically.

    https://github.com/apache/pulsar/pull/7449
    
### Notable Bug Fix

- [Gep Replication] Handle `NoSuchElemetnException` when updating geo replication policy.

    https://github.com/apache/pulsar/pull/7514
    
- [Function] Fix deadlock between create function and leader initialization.

    https://github.com/apache/pulsar/pull/7508
    
- [Broker] Fix get last entry is trying to read entry -1.

    https://github.com/apache/pulsar/pull/7495
    
- [Broker] Fix `ArrayIndexOutOfBoundsException` when dispatch messages to consumer.

    https://github.com/apache/pulsar/pull/7483
    
- [Broker] Avoid the NPE occurs in the method `ManagedLedgerImpl.isOffloadedNeedsDelete`.

    https://github.com/apache/pulsar/pull/7389
    
- [Broker] Fix update partitions error for non-persistent topics.

    https://github.com/apache/pulsar/pull/7459
    
- [Java Client] Fix batch ackset recycled multiple times.

    https://github.com/apache/pulsar/pull/7409

### Event / News

- [Pulsar Summit] The first-ever Pulsar Summit Virtual Conference 2020 was held on June 17 - 18. This two-day digital event featured more than 30 sessions from top Pulsar contributors and developers.

    All video recordings and slides are available at [here](https://streamnative.io/resource#pulsar-summit). 
    
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 015 - What's New in Pulsar 2.6.0 - Sijie Guo

        - Recording: https://www.youtube.com/watch?v=bPczhvnHnzI&list=PLqRma1oIkcWhWAhKgImEeRiQi5vMlqTc-&index=2&t=0s

### Blog / Article

- Pulsar vs. Kafka — Part 1 — A More Accurate Perspective on Performance, Architecture, and Features - Carolyn King, Addison Higham, Sijie Guo

    https://streamnative.io/blog/tech/pulsar-vs-kafka-part-1
