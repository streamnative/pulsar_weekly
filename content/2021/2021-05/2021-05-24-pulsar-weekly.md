---
title: "2021-05-24-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-05-17 ~ 2021-05-23"
date: 2021-05-17 ~ 2021-05-23
description: "This is the Pulsar community weekly update for 2021-05-17 ~ 2021-05-23, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-05-24-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-05-17 ~ 2021-05-23

This is the Pulsar community weekly update for 2021-05-17 ~ 2021-05-23, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Transaction] Support getting the transaction coordinator status through the transaction Admin API.

    https://github.com/apache/pulsar/pull/10639 ([congbobo184](https://api.github.com/users/congbobo184))

### Development

- [Schema] Support consuming messages with multiple schema types through `AutoConsumeSchema`.

    https://github.com/apache/pulsar/pull/10604 ([gaoran10](https://api.github.com/users/gaoran10))

- [BookKeeper] Initialize `ManagedLedgerFactory` with `MetadataStore`.

    https://github.com/apache/pulsar/pull/10647 ([merlimat](https://api.github.com/users/merlimat))

- [Broker] Use the concurrent Hash map to handle locks notifications.

    https://github.com/apache/pulsar/pull/10680 ([merlimat](https://api.github.com/users/merlimat))

- [Pulsar client] Add `org.apache.bookkeeper:cpu-affinity` to the shaded profile.

    https://github.com/apache/pulsar/pull/10681 ([merlimat](https://api.github.com/users/merlimat))

- [BookKeeper] Ensure the `ReadHandle` is properly closed on cache invalidation.

    https://github.com/apache/pulsar/pull/10659 ([merlimat](https://api.github.com/users/merlimat))

- [Broker] Support configuring busy-wait in the Pulsar broker and Pulsar client.

    https://github.com/apache/pulsar/pull/10661 ([merlimat](https://api.github.com/users/merlimat))

- [Broker] Set up transaction metadata with `MetadataStore`.

    https://github.com/apache/pulsar/pull/10677 ([fantapsody](https://api.github.com/users/fantapsody))

- [Broker] Set up initial namespaces with `MetadataStore`.

    https://github.com/apache/pulsar/pull/10612 ([fantapsody](https://api.github.com/users/fantapsody))

- [BookKeeper] Support configuring the number of BookKeeper client worker threads.

    https://github.com/apache/pulsar/pull/10649 ([merlimat](https://api.github.com/users/merlimat))

- [Metrics] Add metrics for the non-contiguous deleted message range.

    https://github.com/apache/pulsar/pull/10638 ([Sunny-Island](https://api.github.com/users/Sunny-Island))

- [Performance] Optimizes the `AuthProviderToken` class to use the same instance of the parser.

    https://github.com/apache/pulsar/pull/10664 ([addisonj](https://api.github.com/users/addisonj))

- [Functions] Process asynchronous results in the same Java runnable thread.

    https://github.com/apache/pulsar/pull/10618 ([sijie](https://api.github.com/users/sijie))

- [Broker] Avoid the context switch when `managedLedgerNewEntriesCheckDelayInMillis` is set to `0`.

    https://github.com/apache/pulsar/pull/10660 ([merlimat](https://api.github.com/users/merlimat))

- [Transaction] Support getting the transaction coordinator status through the transaction Admin API.

    https://github.com/apache/pulsar/pull/10639 ([congbobo184](https://api.github.com/users/congbobo184))

- [Pulsar Admin] Return a better error message.

    https://github.com/apache/pulsar/pull/10628 ([eolivelli](https://api.github.com/users/eolivelli))

- [Java][Schema] Enable disabled tests about `AutoConsume` and `KeyValue` and add the test about null values.

    https://github.com/apache/pulsar/pull/10626 ([eolivelli](https://api.github.com/users/eolivelli))

- [Java][Schema] Add more tests about `KeyValue` and NULL values.

    https://github.com/apache/pulsar/pull/10609 ([eolivelli](https://api.github.com/users/eolivelli))

- [Broker] Set up the Pulsar cluster with `MetadataStore`.

    https://github.com/apache/pulsar/pull/10600 ([fantapsody](https://api.github.com/users/fantapsody))

### Notable Bug Fix

- [Admin] Fix the issue that when getting the partition metadata of a non-existent topic, it returns `0`.

    https://github.com/apache/pulsar/pull/10601 ([BewareMyPower](https://api.github.com/users/BewareMyPower))

- [Admin] Convert the bundle split operation into an HTTP asynchronous operation.

    https://github.com/apache/pulsar/pull/10619 ([merlimat](https://api.github.com/users/merlimat))

- [pulsar-client] Fix the issues in the pulsar-client shading configuration.

    https://github.com/apache/pulsar/pull/10614 ([merlimat](https://api.github.com/users/merlimat))

- [pulsar-client] Fix the issue that the `MessageCrypto` interface should not expose the Netty `ByteBuf` class in the API.

    https://github.com/apache/pulsar/pull/10616 ([merlimat](https://api.github.com/users/merlimat))

- [Build] Fix distribution build errors caused by the denied permission.

    https://github.com/apache/pulsar/pull/10641 ([timmyyuan](https://api.github.com/users/timmyyuan))

- [Test] Fix the failed `TopicPoliciesTest.testMaxSubscriptionsFailFast` test.

    https://github.com/apache/pulsar/pull/10640 ([eolivelli](https://api.github.com/users/eolivelli))

- [Broker] Fix the issue that consumer-related topic stats are only available when the consumer or the reader is connected.

    https://github.com/apache/pulsar/pull/10644 ([dlg99](https://api.github.com/users/dlg99))

- [Common] Fix the `ConcurrentOpenLongPairRangeSet` to remove data for all ranges.

    https://github.com/apache/pulsar/pull/10656 ([315157973](https://api.github.com/users/315157973))

### Event / News

- Pulsar Virtual Summit North America 2021

    - Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

- [Pulsar Office Hour] Monthly live stream about Pulsar best practices, use cases, and more.

  - 05/19: https://www.youtube.com/watch?v=vGg9wiYjvUM

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- What’s New in Apache Pulsar 2.7.2

    - https://streamnative.io/en/blog/release/2021-05-24-pulsar-272

