---
title: "2021-07-05-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-06-28 ~ 2021-07-04"
date: 2021-06-28 ~ 2021-07-04
description: "This is the Pulsar community weekly update for 2021-06-28 ~ 2021-07-04, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-07-05-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-06-28 ~ 2021-07-04

This is the Pulsar community weekly update for 2021-06-28 ~ 2021-07-04, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- PIP-45: Convert the bookies REST endpoint to use the metadata store.

  https://github.com/apache/pulsar/pull/11210 ([@merlimat](https://github.com/merlimat))
  
### Development

- PIP 85: Expose the Pulsar Client via the Pulsar Functions and Pulsar connector `BaseContext`.

 https://github.com/apache/pulsar/wiki/PIP-85%3A-Expose-Pulsar-Client-via-Function-Connector-BaseContext ([@nlu90](https://github.com/nlu90))

### Notable Feature

- [Tiered Storage] Remove unused listeners to avoid creating the executor pool.

  https://github.com/apache/pulsar/pull/11215 ([@Technoboy-](https://github.com/Technoboy-))
  
- [Broker] Support configuring the execution time of the compaction phase one loop.

  https://github.com/apache/pulsar/pull/11206 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Adjust the implementation of `getDynamicConfigurationDouble` and `DynamicConfigurationBoolean`.

  https://github.com/apache/pulsar/pull/11171 ([@Technoboy-](https://github.com/Technoboy-))
  
- [Website] Add a local debugging tool for viewing Pulsar website updates.

  https://github.com/apache/pulsar/pull/11160 ([@urfreespace](https://github.com/urfreespace))
  
- [Broker] Add an authoritative flag for the topic-level policy to avoid the redirect loop.

  https://github.com/apache/pulsar/pull/11131 ([@codelipenghui](https://github.com/codelipenghui))
  
- [Broker] Clear redundant codes.

  https://github.com/apache/pulsar/pull/11071 ([@linlinnn](https://github.com/linlinnn))
  
- [Test] Use `Awaitility to` instead of `Thread sleep`.

  https://github.com/apache/pulsar/pull/11164 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker/Bookie] Set `-Dio.netty.tryReflectionSetAccessible=true` for Pulsar processes.

  https://github.com/apache/pulsar/pull/11138 ([@lhotari](https://github.com/lhotari))
  
- [Test] Add a new test for `MaxRequestSizeFilter`.

  https://github.com/apache/pulsar/pull/11128 ([@mattisonchao](https://github.com/mattisonchao))
  
- [Test] Add a new test for `ProcessHandlerFilter`.

  https://github.com/apache/pulsar/pull/11133 ([@mattisonchao](https://github.com/mattisonchao))

### Notable Bug Fix

- [Broker] Fix the compaction entry read exception.

  https://github.com/apache/pulsar/pull/11175 ([@hangc0276](https://github.com/hangc0276))

- [Broker] Fix the issue that the `CommandSubscribe.getConsumerName()` is used without checking whether the consumer name is set.

  https://github.com/apache/pulsar/pull/11199 ([@merlimat](https://github.com/merlimat))

- [Broker] Fix the possible deadlock in the initialization of `MLTransactionLog`.

  https://github.com/apache/pulsar/pull/11194 ([@merlimat](https://github.com/merlimat))

- [Test] Fix the failed authentication test.

  https://github.com/apache/pulsar/pull/11186 ([@sursingh](https://github.com/sursingh))

- [Broker] Fix the deadlock when using `hasMessageAvailableAsync` and `readNextAsync`.

  https://github.com/apache/pulsar/pull/11183 ([@codelipenghui](https://github.com/codelipenghui))

- [Test] Provide minor refactor for `ZookeeperServerTest`.

  https://github.com/apache/pulsar/pull/11181 ([@yangl](https://github.com/yangl))

- [C++ client] Fix the regex namespace to avoid the core dump.

  https://github.com/apache/pulsar/pull/11179 ([@cimura](https://github.com/cimura))

- [Test] Fix the copy-paste error in the test.

  https://github.com/apache/pulsar/pull/11176 ([@mattisonchao](https://github.com/mattisonchao))

- [Functions] Fix some incorrect usage methods.

  https://github.com/apache/pulsar/pull/11167 ([@mattisonchao](https://github.com/mattisonchao))

- [C++] Fix the missed header for some compilers.

  https://github.com/apache/pulsar/pull/11152 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Test] Fix the `LoadBalancerTest.testBrokerRanking` Flaky test.

  https://github.com/apache/pulsar/pull/11150 ([@Technoboy-](https://github.com/Technoboy-))

- [Broker] Fix the issue that the topic-level retention policy does not work.

  https://github.com/apache/pulsar/pull/11136 ([@hangc0276](https://github.com/hangc0276))

- [Test] Change the test group to the broker for `ReplicatorTest` and fix the test.

  https://github.com/apache/pulsar/pull/11134 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the issue that the subscription permission does not work in the reset cursor.

  https://github.com/apache/pulsar/pull/11132 ([@wuzhanpeng](https://github.com/wuzhanpeng))

- [C++] Fix the boost download link in the `Dockerfile`.

  https://github.com/apache/pulsar/pull/11129 ([@sh05](https://github.com/sh05))

- [Test] Fix the `TopicFromMessageTest.testMultiTopicConsumerBatchShortName` Flaky test.

  https://github.com/apache/pulsar/pull/11125 ([@Technoboy-](https://github.com/Technoboy-))

- [Broker] Fix the timestamp description for `resetCursor`.

  https://github.com/apache/pulsar/pull/11121 ([@bem3](https://github.com/bem3))

- [Test] Fix the incorrect `TimeUnit`.

  https://github.com/apache/pulsar/pull/11118 ([@mattisonchao](https://github.com/mattisonchao))

- [Test] Fix the `testBrokerRanking` Flaky test.

  https://github.com/apache/pulsar/pull/11114 ([@hangc0276](https://github.com/hangc0276))

- [Pulsar-IO] Fix `SinkConfig.inputs` to return a list of topics.

  https://github.com/apache/pulsar/pull/11094 ([@murong00](https://github.com/murong00))

- [Broker] Fix the issue that the `publish_time` is not set when the broker entry metadata is enabled without `AppendBrokerTimestampMetadataInterceptor`.

  https://github.com/apache/pulsar/pull/11014 ([@aloyszhang](https://github.com/aloyszhang))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Announcing Pulsar Virtual Summit Europe 2021: CFP Is Open!

    - https://streamnative.io/en/blog/community/2021-06-30-announcing-pulsar-virtual-summit-europe-2021-cfp-is-open
