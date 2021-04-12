---
title: "2021-04-12-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-04-05 ~ 2021-04-11"
date: 2021-04-05 ~ 2021-04-11
description: "This is the Pulsar community weekly update for 2021-04-05 ~ 2021-04-11, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-04-12-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-04-05 ~ 2021-04-11

This is the Pulsar community weekly update for 2021-04-05 ~ 2021-04-11, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

[Schema Registry] Introduce a new high-level `GenericObject` interface that represents every logic value on the Pulsar topic. It supports writing sinks that work with every Schema type.

by (@[eolivelli](https://github.com/eolivelli))

### Development

- [PIP-82] [Broker] Add a task to publish resource usage to a topic.

    https://github.com/apache/pulsar/pull/10008 (@[bharanic-dev](https://github.com/bharanic-dev))

### Notable Feature

- [Test] Refactor existing Pulsar Function unit tests.

    https://github.com/apache/pulsar/pull/10125 (@[david-streamlio](https://github.com/david-streamlio))

- [C++] Support configuring the memory limit from the C++ API.

    https://github.com/apache/pulsar/pull/10145 (@[merlimat](https://github.com/merlimat))

- [Functions] Expose Prometheus metrics for Pulsar functions in the local-run mode.

    https://github.com/apache/pulsar/pull/10156 (@[jerrypeng](https://github.com/jerrypeng))

- [Schema Registry] Implement `GenericObject`, which allows `GenericRecord` to wrap any Java object.

    https://github.com/apache/pulsar/pull/10057 (@[eolivelli](https://github.com/eolivelli))

- [Admin] Support setting namespace-level and topic-level policies for the non-persistent dispatcher.

    https://github.com/apache/pulsar/pull/10121 (@[315157973](https://github.com/315157973))

- [C++] Add `/opt/homebrew/` as a possible path for OpenSSL on Mac OS.

    https://github.com/apache/pulsar/pull/10141 (@[merlimat](https://github.com/merlimat))

- [Schema Registry] Support `KeyValue` in `Message#getValue()`.

    https://github.com/apache/pulsar/pull/10107 (@[eolivelli](https://github.com/eolivelli))

- [IO] Support developing sinks that support Schema but do not set Schema at the build time.

    https://github.com/apache/pulsar/pull/10034 (@[eolivelli](https://github.com/eolivelli))

### Notable Bug Fix

- [Client] Fix the issue that `ClientConfigurationData`'s objects are not effectively equal.

    https://github.com/apache/pulsar/pull/10091 (@[dlg99](https://github.com/dlg99))

- [Transaction] Fix the NPE that occurs if transactions are not enabled when you try to create a transaction.

    https://github.com/apache/pulsar/pull/10139 (@[linlinnn](https://github.com/linlinnn))

- [Broker] Fix the issue that some partitions are stuck when additional consumers are added in the Key_shared subscription mode.

    https://github.com/apache/pulsar/pull/10096 (@[baomingyu](https://github.com/baomingyu))

- [Transaction] Fix the issue that the transaction log cannot be recovered.

    https://github.com/apache/pulsar/pull/10146 (@[congbobo184](https://github.com/congbobo184))

- [Transaction] Fix the issue that occurs when aborting the transaction retry.

    https://github.com/apache/pulsar/pull/10131 (@[congbobo184](https://github.com/congbobo184))

- [Broker] Fix the the issue that the consumer is blocked after receiving retry messages many times if the consumer enables the retry feature and sets the retry topic in `DeadLetterPolicy`.

    https://github.com/apache/pulsar/pull/10078 (@[gaoran10](https://github.com/gaoran10))

- [Flaky Test] Fix the `SimpleProducerConsumerTestStreamingDispatcherTest.testRedeliveryFailOverConsumer` flaky test.

    https://github.com/apache/pulsar/pull/10118 (@[lhotari](https://github.com/lhotari))

- [C++] Fix the race condition in `MemoryLimitController`.

    https://github.com/apache/pulsar/pull/10142 (@[merlimat](https://github.com/merlimat))

- [C++] Fix the issue that the C++ client fails to release the semaphore and reserved memory in case of send timeouts.

    https://github.com/apache/pulsar/pull/10144 (@[merlimat](https://github.com/merlimat))

- [Broker] Fix the `IllegalStateException` exception in `PersistentReplicator`.

    https://github.com/apache/pulsar/pull/10098 (@[lhotari](https://github.com/lhotari))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- Apache Pulsar Hackathon

    Sign-up: https://www.eventbrite.com/e/apache-pulsar-hackathon-2021-tickets-143906003731

- Pulsar Virtual Summit North America 2021

    Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

### Blog / Article

- Function Mesh Now Available for Pulsar Functions

    - https://streamnative.io/en/blog/release/2021-04-05-function-mesh-now-available-for-pulsar-functions