---
title: "2020-11-20-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-11-14 ~ 2020-11-20"
date: 2020-11-14 ~ 2020-11-20
description: "This is the Pulsar community weekly update for 2020-11-14 ~ 2020-11-20, with updates on Pulsar client, broker, transaction, Functions, schema, Pulsar IO, and so on."
id: "2020-11-20-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-11-14 ~ 2020-11-20

This is the Pulsar community weekly update for 2020-11-14 ~ 2020-11-20, with updates on Pulsar client, broker, transaction, Functions, schema, Pulsar IO, and so on.

### Pulsar Highlight

Support the Protobuf Native Schema. Before this PR, `ProtobufSchema` was based on the AVRO schema which has some restrictions. For details, see [PR-8372](https://github.com/apache/pulsar/pull/8372).

by (@[hnail](https://github.com/hnail))

### Notable Feature

- [BookKeeper] Upgrade BookKeeper to version 4.12.0.

    https://github.com/apache/pulsar/pull/8447 (@[eolivelli](https://github.com/eolivelli))

- [Client] Add the smoke test for the shade package.

    https://github.com/apache/pulsar/pull/8574 (@[reswqa](https://github.com/reswqa))

- [Broker] Support setting the topic-level `DeduplicationSnapshotInterval`.

    https://github.com/apache/pulsar/pull/8552 (@[315157973](https://github.com/315157973))

- [Function] Support the key_based batch builder for Functions and sources.

    https://github.com/apache/pulsar/pull/8523 (@[wolfstudy](https://github.com/wolfstudy))

- [Broker] Add the key-shared consumer range to internal topic stats.

    https://github.com/apache/pulsar/pull/8567 (@[MarvinCai](https://github.com/MarvinCai))

- [Pulsar IO] Add `passive` to the RabbitMQ IO configuration options.

    https://github.com/apache/pulsar/pull/8075 (@[seeday](https://github.com/seeday))

- [Client] Support partitioned topics in the reader.

    https://github.com/apache/pulsar/pull/7518 (@[315157973](https://github.com/315157973))

- [Function] Support Kubernetes runtime for Go Functions.

    https://github.com/apache/pulsar/pull/8352 (@[freeznet](https://github.com/freeznet))

- [Schema Registry] Support the Protobuf Native Schema.

    https://github.com/apache/pulsar/pull/8372 (@[hnail](https://github.com/hnail))

- [Broker] Close topics that are fenced forcefully.

    https://github.com/apache/pulsar/pull/8561 (@[massakam](https://github.com/massakam))

- [Transaction] Guarantee transaction metadata handlers to be connected with the broker.

    https://github.com/apache/pulsar/pull/8563 (@[gaoran10](https://github.com/gaoran10))

- [Broker] Make the `ServerCnx` that is used by the producer and consumer independent from Netty.

    https://github.com/apache/pulsar/pull/6720 (@[cbornet](https://github.com/cbornet))

- [Schema Registry] Support decoding multi-version reader to ensure users custom the reader to decode multi-version messages.

    https://github.com/apache/pulsar/pull/8464 (@[congbobo184](https://github.com/congbobo184))

- [Transaction] Add the transaction integration test.

    https://github.com/apache/pulsar/pull/8594 (@[gaoran10](https://github.com/gaoran10))

- [Pulsar IO] Add the NSQ Source.

    https://github.com/apache/pulsar/pull/8250 (@[flowchartsman](https://github.com/flowchartsman))

- [Go Functions] Access to user configuration before the Function loop.

    https://github.com/apache/pulsar/pull/8467 (@[flowchartsman](https://github.com/flowchartsman))

- [Broker] Improve the performance of `checkPublishRate()`.

    https://github.com/apache/pulsar/pull/8623 (@[wangjialing218](https://github.com/wangjialing218))

- [Managed Ledger] Perform periodic flush of `ManagedCursor` mark-delete positions.

    https://github.com/apache/pulsar/pull/8634/files (@[merlimat](https://github.com/merlimat))

- [Transaction] Support sending transaction messages synchronously.

    https://github.com/apache/pulsar/pull/8631 (@[gaoran10](https://github.com/gaoran10))

- [Proxy] Support enabling WebSocket on the Pulsar Proxy.

    https://github.com/apache/pulsar/pull/8613 (@[codelipenghui](https://github.com/codelipenghui))

- [Function] Enable Pulsar Function to send message to external Pulsar clusters.

    https://github.com/apache/pulsar/pull/8434 (@[nlu90](https://github.com/nlu90))

### Notable Bug Fix

- [C++] Fix flaky tests of `KeySharedConsumerTest`.

    https://github.com/apache/pulsar/pull/8568 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Transaction] Fix the Github CI test.

    https://github.com/apache/pulsar/pull/8541 (@[congbobo184](https://github.com/congbobo184))

- [Broker] Fix the issue that the managed-ledger `addEntry-latency` bucket stats are measured per minute.

    https://github.com/apache/pulsar/pull/8218 (@[rdhabalia](https://github.com/rdhabalia))

- [Broker] Fix the incorrect add-entry latency.

    https://github.com/apache/pulsar/pull/8219 (@[rdhabalia](https://github.com/rdhabalia))

- [SQL] Fix the issue that Pulsar SQL cannot query the last message.

    https://github.com/apache/pulsar/pull/8635 (@[zymap](https://github.com/zymap))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

### Blog / Article

- Pulsar Advantages Over Kafka -- Javier Ramos

  - https://itnext.io/pulsar-advantages-over-kafka-7e0c2affe2d6
