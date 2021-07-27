---
title: "2021-07-26-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-07-19 ~ 2021-07-25"
date: 2021-07-19 ~ 2021-07-25
description: "This is the Pulsar community weekly update for 2021-07-19 ~ 2021-07-25, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-07-26-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-07-19 ~ 2021-07-25

This is the Pulsar community weekly update for 2021-07-19 ~ 2021-07-25, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Broker] PIP-82: Update the resource-group stats.

    https://github.com/apache/pulsar/pull/11331 ([kaushik-develop](https://github.com/kaushik-develop))

- [C++ Client] Support the Protobuf native schema.

    https://github.com/apache/pulsar/pull/11388 ([BewareMyPower](https://github.com/BewareMyPower))

### Notable Feature

- [Broker] Support setting multiples roles for authorization.

    https://github.com/apache/pulsar/pull/11341 ([RobertIndie](https://github.com/RobertIndie))

- [Python Client] Support the complex schema.

    https://github.com/apache/pulsar/pull/11400 ([gaoran10](https://github.com/gaoran10))

- [Pulsar IO] Allow Pulsar IO sink connectors to use the native AVRO and JSON formats.

    https://github.com/apache/pulsar/pull/11322 ([eolivelli](https://github.com/eolivelli))

- [Monitor] Add the `storageLogicalSize` metric to the `TopicStats` and `NamespaceStats`.

    https://github.com/apache/pulsar/pull/11430 ([Technoboy-](https://github.com/Technoboy-))

- [Broker] Close the replicator and replication client when deleting a Pulsar cluster.

    https://github.com/apache/pulsar/pull/11342 ([codelipenghui](https://github.com/codelipenghui))

### Notable Bug Fix

- [CLI] Fix the issue in the pulsar-admin CLI tool when validating the batch source configuration.

    https://github.com/apache/pulsar/pull/11378 ([jerrypeng](https://github.com/jerrypeng))

- [Admin] Fix the issue that only subscriptions created for `Partition-0` are listed when partition-specific subscriptions are created.

    https://github.com/apache/pulsar/pull/11355 ([Technoboy-](https://github.com/Technoboy-))

- [Function] Reduce the probability of cache inconsistencies.

    https://github.com/apache/pulsar/pull/11423 ([315157973](https://github.com/315157973))

- [Transaction] Fix the direct memory leak related to the commit and abort markers.

    https://github.com/apache/pulsar/pull/11407 ([lhotari](https://github.com/lhotari))

- [Client] Avoid waiting infinitely when closing a consumer.

    https://github.com/apache/pulsar/pull/11347 ([Shoothzj](https://github.com/Shoothzj))

- [Broker] Delete the topic-level policies after deleting a topic.

    https://github.com/apache/pulsar/pull/11316 ([horizonzy](https://github.com/horizonzy))

- [Python Function] Fix the issue that the `tls_validate_hostname` is not supported in the Python Functions runtime.

    https://github.com/apache/pulsar/pull/11087 ([freeznet](https://github.com/freeznet))

- [C++ Client] Use the same regex code at `ZTSClient`.

    https://github.com/apache/pulsar/pull/11323 ([equanz](https://github.com/equanz))

- [Broker] Fix the issue that the broker leaks direct memory when using replicated subscriptions and Key_Shared consumers.

    https://github.com/apache/pulsar/pull/11396 ([lhotari](https://github.com/lhotari))

- [Broker] Fix the NPE that occurs when the builtin connectors do not exist.

    https://github.com/apache/pulsar/pull/11385 ([jerrypeng](https://github.com/jerrypeng))

### Ecosystem

- [Connector] Support multiple Elasticsearch hosts.

    https://github.com/apache/pulsar/pull/10973 ([wangjialing218](https://github.com/wangjialing218))

- [Pulsar IO] Ensure that the `ack()` method of the `AbstractKafkaSourceRecord` is not blocking to avoid deadlock.

    https://github.com/apache/pulsar/pull/11435 ([nlu90](https://github.com/nlu90))

- [NiFi] Fix the concurrency issues in NarUnpacker.

    https://github.com/apache/pulsar/pull/11343 ([lhotari](https://github.com/lhotari))

### Event / News

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

### Blog / Article

- Join Us to Organize Your Local Apache Pulsar 2.8.0 Release Party

    - https://streamnative.io/en/blog/community/2021-07-16-release-party

- Apache Pulsar Launches 2.8: Unified Messaging and Streaming With Transactions

    - https://medium.com/streamnative/apache-pulsar-launches-2-8-unified-messaging-and-streaming-with-transactions-37dad479cba1