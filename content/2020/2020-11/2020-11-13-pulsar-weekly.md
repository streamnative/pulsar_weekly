---
title: "2020-11-13-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-11-07 ~ 2020-11-13"
date: 2020-11-07 ~ 2020-11-13
description: "This is the Pulsar community weekly update for 2020-11-07 ~ 2020-11-13, with updates on Pulsar client, broker, transaction, WebSocket, and so on."
id: "2020-11-13-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-11-07 ~ 2020-11-13

This is the Pulsar community weekly update for 2020-11-07 ~ 2020-11-13, with updates on Pulsar client, broker, transaction, WebSocket, and so on.

### Pulsar Highlight

Expose the transaction client interface. For details, see [PR-8505](https://github.com/apache/pulsar/pull/8505).

by (@[congbobo184](https://github.com/congbobo184))

### Development

- PIP-72: Introduce the Pulsar Interface Taxonomy for audience and stability classification.

	https://github.com/apache/pulsar/pull/8530 (@[sijie](https://github.com/sijie))

- PIP-38: Support batching receive in Java client.

    https://github.com/apache/pulsar/pull/4621 (@[codelipenghui](https://github.com/codelipenghui))

### Notable Feature

- [Functions] Refactor Context and State API to allow plugging different state store implementations.

	https://github.com/apache/pulsar/pull/8537 (@[sijie](https://github.com/sijie))

- [Broker] Expose consumer names after the mark delete position for the Key_Shared subscription.

    https://github.com/apache/pulsar/pull/8545 (@[codelipenghui](https://github.com/codelipenghui))

- [Websocket] Support WebSocket producer for V2 topics.

    https://github.com/apache/pulsar/pull/8535 (@[k2la](https://github.com/k2la))

- [Transaction] Register transaction metadata before sending or acknowledging messages.

    https://github.com/apache/pulsar/pull/8493 (@[gaoran10](https://github.com/gaoran10))

- [Transaction] Expose the transaction interface.

    https://github.com/apache/pulsar/pull/8505 (@[congbobo184](https://github.com/congbobo184))

- [Functions] Improve the Function state workflow with timeouts.

    https://github.com/apache/pulsar/pull/8528 (@[jerrypeng](https://github.com/jerrypeng))

- [Client] The Java client supports `UnAvroBased` Schema.

    https://github.com/apache/pulsar/pull/8246 (@[hnail](https://github.com/hnail))

- [Broker] Support disabling replicated subscriptions.

    https://github.com/apache/pulsar/pull/8144 (@[k2la](https://github.com/k2la))

- [Transaction] Support pending-ack state for batch messages and implement pending-ack server patch.

    https://github.com/apache/pulsar/pull/8426 (@[congbobo184](https://github.com/congbobo184))

- [Client] Add ability to examine specific messages based on the position related to the earliest or the latest message.

    https://github.com/apache/pulsar/pull/8494 (@[MarvinCai](https://github.com/MarvinCai))

- [Broker] Improve the test code readability and maintainability by refactoring repeated values.

    https://github.com/apache/pulsar/pull/8052 (@[kellyfj](https://github.com/kellyfj))

- [Functions] Asynchronously run the batch source discovery and acknowledge task messages.

    https://github.com/apache/pulsar/pull/8498 (@[jerrypeng](https://github.com/jerrypeng))

- [Client] Update the `getBrokersWithNamespaceIsolationPolicy` command.

    https://github.com/apache/pulsar/pull/8472 (@[jiazhai](https://github.com/jiazhai))

- [Broker] Support taking de-duplication snapshots based on time.

    https://github.com/apache/pulsar/pull/8474 (@[315157973](https://github.com/315157973))

- [Function] Enable E2E encryption for Pulsar Function.

    https://github.com/apache/pulsar/pull/8432 (@[nlu90](https://github.com/nlu90))

### Notable Bug Fix

- [Functions] Fix the issue that when overriding `jobName` in Kubernetes runtime with custom runtime options can have collisions when same `jobName` is used.

    https://github.com/apache/pulsar/pull/8508 (@[jdbeck](https://github.com/jdbeck))

- [Broker] Fix the issue that when using `inactivityMonitor` command to clean inactive partitioned topic, the node in ZooKeeper is not deleted.

    https://github.com/apache/pulsar/pull/8442 (@[315157973](https://github.com/315157973))

- [Client] Fix the typo in pulsar-client-all module's pom.xml.

    https://github.com/apache/pulsar/pull/8543(@[reswqa](https://github.com/reswqa))

- [Transaction] Fix the `TransactionBufferHandlerImpl` thread leak in tests.

    https://github.com/apache/pulsar/pull/8488(@[eolivelli] (https://github.com/eolivelli))

- [Client] Fix race condition when calling `acknowledgementWasProcessed()`.

    https://github.com/apache/pulsar/pull/8499(@[codelipenghui] (https://github.com/codelipenghui))

- [Client] Fix handling errors for client requests.

    https://github.com/apache/pulsar/pull/8518 (@[merlimat](https://github.com/merlimat))

- [C++] Fix the potential crash caused by the AckGroupTracker's timer.

    https://github.com/apache/pulsar/pull/8519 (@[BewareMyPower](https://github.com/BewareMyPower))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

### Blog / Article

- Event-driven railway network based on Pulsar -- Pavels Sisojevs

  - https://streamnative.io/blog/release/2020-10-28-streamnative-free-cloud

- Powering Federated Learning at Tencent with Apache Pulsar

  - https://streamnative.io/success-stories/tencent-angel

- Benchmarking Pulsar and Kafka - A More Accurate Perspective on Pulsar’s Performance

  - https://streamnative.io/blog/tech/2020-11-09-benchmark-pulsar-kafka-performance

- Benchmarking Pulsar and Kafka - The Full Benchmark Report

  - https://streamnative.io/blog/tech/2020-11-09-benchmark-pulsar-kafka-performance-report

- Apache Pulsar 2.6.2

  - https://pulsar.apache.org/blog/2020/11/09/Apache-Pulsar-2-6-2/