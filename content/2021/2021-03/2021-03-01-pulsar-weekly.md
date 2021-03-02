---
title: "2021-03-01-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-02-22 ~ 2021-02-28"
date: 2021-02-22 ~ 2021-02-28
description: "This is the Pulsar community weekly update for 2021-02-22 ~ 2021-02-28, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-03-01-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-02-22 ~ 2021-02-28

This is the Pulsar community weekly update for 2021-02-22 ~ 2021-02-28, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Notable Feature

- Support getting the topic-applied policy for `DeduplicationStatus`.

    https://github.com/apache/pulsar/pull/9339 ([@315157973](https://github.com/315157973))

- [Client] Make function dependencies as optional components for the Pulsar Python client.

    https://github.com/apache/pulsar/pull/9719 ([@aahmed-se](https://github.com/aahmed-se))

- [Metrics] Reduce CPU consumption of metrics creation.

    https://github.com/apache/pulsar/pull/9735 ([@lhotari](https://github.com/lhotari))

- [Metrics] Add metrics for producer throttling.

    https://github.com/apache/pulsar/pull/9649 ([@merlimat](https://github.com/merlimat))

- [Client] Refactor seek to reuse the common logic.

    https://github.com/apache/pulsar/pull/9670 ([@sunxiaoguang](https://github.com/sunxiaoguang))

- [Compression] Fix `ByteBuffer` allocated error in the `AirliftUtils`.

    https://github.com/apache/pulsar/pull/9667 (@[gaoran10](https://github.com/gaoran10))

- [Client] Expose `ReachedEndOfTopic` in the Reader/Consumer API.

    https://github.com/apache/pulsar/pull/9381 ([@MarvinCai](https://github.com/MarvinCai))

- [Build] Add Java 11 to Pulsar build image and upgrade dependencies.

    https://github.com/apache/pulsar/pull/9609 ([@eolivelli](https://github.com/eolivelli))

### Notable Bug Fix

- [Release] Fix the issue with marking individual deletes as dirty.

    https://github.com/apache/pulsar/pull/9732 (@[addisonj](https://github.com/addisonj))

- [Release] Keep the style of `max-subscriptions` command consistent.

    https://github.com/apache/pulsar/pull/9750 ([@315157973](https://github.com/315157973))

- [Transaction] Fix `deleteTransactionMarker` memory leak.

    https://github.com/apache/pulsar/pull/9751 ([@michaeljmarshall](https://github.com/michaeljmarshall))

- [Client] Remove the message data size messages get out of the queue.

    https://github.com/apache/pulsar/pull/8566 ([@MaiCw4J](https://github.com/MaiCw4J))

- [[Broker] Fix the issue that automatic topic compaction is never triggered if no durable subscriptions are found.

    https://github.com/apache/pulsar/pull/8204 ([@fmiguelez](https://github.com/fmiguelez))

- [C++] Fix the issue that `SinglePartitionMessageRouter` always picks the same partition.

    https://github.com/apache/pulsar/pull/9702 ([@merlimat](https://github.com/merlimat))

- [Test] Add debugging feature which leaves integration test containers running after the test is completed.

    https://github.com/apache/pulsar/pull/9626 [@lhotari](https://github.com/lhotari)

- [Release] Use the atomic field updater to increment volatile `messagesConsumedCounter`.

    https://github.com/apache/pulsar/pull/9656 ([@aahmed-se](https://github.com/aahmed-se))

### Ecosystem

- [Pulsar SQL] Fix the Pulsar SQL query bytes schema data error.

    https://github.com/apache/pulsar/pull/9631 (@[gaoran10](https://github.com/gaoran10))

- [Pulsar SQL] Fix the duplicated __pfn_input_topic__ key in the Presto server.

    https://github.com/apache/pulsar/pull/9686 ([@pointearth](https://github.com/pointearth))

- [Pulsar SQL] Add the test for Pulsar SQL to support `keyValue` schema.

    https://github.com/apache/pulsar/pull/9388 ([@congbobo184](https://github.com/congbobo184))

- [Metrics] Add metrics for the persistence of cursor acknowledgement state.

    https://github.com/apache/pulsar/pull/9618 ([@limingnihao](hhttps://github.com/limingnihao))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - https://www.youtube.com/watch?v=Hp9m-O9f9yo

### Blog / Article

- Pulsar Summit North America 2021: CFP Open Now!

    - https://streamnative.io/en/blog/community/2021-02-23-pulsar-summit-north-america-2021-cfp-open-now
