---
title: "2022-03-07-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-02-28 ~ 2022-03-06"
date: 2022-02-28 ~ 2022-03-06
description: "This is the Pulsar community weekly update for 2022-02-28 ~ 2022-03-06, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-03-07-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-02-28 ~ 2022-03-07

This is the Pulsar community weekly update for 2022-02-28 ~ 2022-03-06, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[mattisonchao](https://github.com/mattisonchao), [fantapsody](https://github.com/fantapsody), [aloyszhang](https://github.com/aloyszhang), [lhotari](https://github.com/lhotari), [freeznet](https://github.com/freeznet), [lordcheng10](https://github.com/lordcheng10), [Zod705](https://github.com/Zod705), [shibd](https://github.com/shibd), [alicebi-streamnative](https://github.com/alicebi-streamnative), [yuruguo](https://github.com/yuruguo), [momo-jun](https://github.com/momo-jun), [nicoloboschi](https://github.com/nicoloboschi), [Anonymitaet](https://github.com/Anonymitaet), [fanla2021](https://github.com/fanla2021), [tuhaihe](https://github.com/tuhaihe), [Demogorgon314](https://github.com/Demogorgon314), [rdhabalia](https://github.com/rdhabalia), [eolivelli](https://github.com/eolivelli), [gaozhangmin](https://github.com/gaozhangmin)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Highlights
- [Broker] Optimize memory usage.
  <br>https://github.com/apache/pulsar/pull/14515 
  <br>by [lordcheng10](https://github.com/lordcheng10)

### Notable Features
- [Pulsar IO] Support event-time-based index name in the ES Sink.
  <br>https://github.com/apache/pulsar/pull/14383 
  <br>by [fantapsody](https://github.com/fantapsody)
- [Broker] Let `standalone` use `setMetadataStoreUrl`.
  <br>https://github.com/apache/pulsar/pull/14384 
  <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Broker] Optimize memory usage.
  <br>https://github.com/apache/pulsar/pull/14515 
  <br>by [lordcheng10](https://github.com/lordcheng10)
- [Java Client] Add timeout to `closeAsync`.
  <br>https://github.com/apache/pulsar/pull/14538 
  <br>by [lhotari](https://github.com/lhotari)
- [Broker] Role with namespace `produce` or `consume` AuthZ can get topics.
  <br>https://github.com/apache/pulsar/pull/13773 
  <br>by [yuruguo](https://github.com/yuruguo)

### Notable Bug Fix
- [Broker] Fix race conditions in the `/brokers/health` endpoint. 
 <br>https://github.com/apache/pulsar/pull/14367 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Test] Fix the Flaky-est `AdminApiTest.testNamespaceSplitBundleConcurrent`.
 <br>https://github.com/apache/pulsar/pull/14565 
 <br>by [aloyszhang](https://github.com/aloyszhang)
- [Functions] Pass configured `metricsPort` to K8S Runtime.
 <br>https://github.com/apache/pulsar/pull/14502 
 <br>by [lhotari](https://github.com/lhotari)
- [Pulsar IO] Throw exceptions when Kafka offset backing store fails to start.
 <br>https://github.com/apache/pulsar/pull/14491 
 <br>by [freeznet](https://github.com/freeznet)
- [Transaction] Fix `topicTransactionBuffer`.
 <br>https://github.com/apache/pulsar/pull/14510 
 <br>by [eolivelli](https://github.com/eolivelli)
- [Transaction] Fix the issue that `MLTransactionMetadataStore.update` async fails.
 <br>https://github.com/apache/pulsar/pull/14532 
 <br>by [shibd](https://github.com/shibd)
- [Test] Fix the flaky test `BrokerBkEnsemblesTests.testCrashBrokerWithoutCursorLedgerLeak`.
 <br>https://github.com/apache/pulsar/pull/14519 
 <br>by [shibd](https://github.com/shibd)
- [Transaction] Fix thread leaks in `MLTransactionMetadataStore`.
 <br>https://github.com/apache/pulsar/pull/14524 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Fix the issue that invoking the `join()` method can cause some deadlocks.
 <br>https://github.com/apache/pulsar/pull/14469 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Tests] Let the test JVM exit if OOME occurs.
 <br>https://github.com/apache/pulsar/pull/14509 
 <br>by [lhotari](https://github.com/lhotari)
- [Tests] Add a retry mechanism to assert `getIfCached`.
 <br>https://github.com/apache/pulsar/pull/14373 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [BookKeeper] Support shrink in `ConcurrentLongHashMap`.
 <br>https://github.com/apache/pulsar/pull/14497 
 <br>by [lordcheng10](https://github.com/lordcheng10)

## Blog
- [Generating Simulated Streaming Data](https://dzone.com/articles/generating-simulated-streaming-data)

## Events / News
- Upcoming events
    - 8 April, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - 17 May, 2022: Kubernetes Batch + HPC Day Europe
        - [Fast Data on-Ramp with Apache Pulsar on K8](https://kubernetesbatchdayeu22.sched.com/event/10F0q)
    - 18-20 July, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
