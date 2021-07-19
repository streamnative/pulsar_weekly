---
title: "2021-07-19-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-07-12 ~ 2021-07-18"
date: 2021-07-12 ~ 2021-07-18
description: "This is the Pulsar community weekly update for 2021-07-12 ~ 2021-07-18, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-07-19-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-07-12 ~ 2021-07-18

This is the Pulsar community weekly update for 2021-07-12 ~ 2021-07-18, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Security] Bump Netty to version `4.1.66.Final`.

    https://github.com/apache/pulsar/pull/11344 ([lhotari](https://github.com/lhotari))

### Notable Feature

- [Security] Bump Netty to version `4.1.66.Final`.

    https://github.com/apache/pulsar/pull/11344 ([lhotari](https://github.com/lhotari))

- [C++] Use the same regex code at `ZTSClient`.

    https://github.com/apache/pulsar/pull/11323 ([equanz](https://github.com/equanz))

- [Broker] Close the replicator and replication client when deleting clusters.

    https://github.com/apache/pulsar/pull/11342 ([codelipenghui](https://github.com/codelipenghui))

- [Go Functions] Set the subscription name for the Go function runtime.

    https://github.com/apache/pulsar/pull/11332 ([nlu90](https://github.com/nlu90))

- [Go Functions] Upgrade the Go client to version 0.5.0.

    https://github.com/apache/pulsar/pull/11336 ([wolfstudy](https://github.com/wolfstudy))

- [pulsar-perf] Add missing parameters for pulsar-perf CLI commands.

    https://github.com/apache/pulsar/pull/11337 ([wolfstudy](https://github.com/wolfstudy))

- [C++] Avoid throwing exceptions when setting the socket option.

    https://github.com/apache/pulsar/pull/11329 ([BewareMyPower](https://github.com/BewareMyPower))

- [BookKeeper] Remove duplicated configurations.

    https://github.com/apache/pulsar/pull/11283 ([aloyszhang](https://github.com/aloyszhang))

- [C++] Support building a debug version of Pulsar C++ library on the Windows operation system.

    https://github.com/apache/pulsar/pull/11302 ([BewareMyPower](https://github.com/BewareMyPower))

- [Pulsar Dashboard] Remove the Pulsar Dashboard.

    https://github.com/apache/pulsar/pull/11284 ([eolivelli](https://github.com/eolivelli))

- [Admin] Expose more attributes of messages to Admin CLI get message information by using `peekMessage` or `getMessageById`.

    https://github.com/apache/pulsar/pull/11279 ([aloyszhang](https://github.com/aloyszhang))

### Notable Bug Fix

- [Common] Fix inconsistent behavior for the cache of namespace bundles.

    https://github.com/apache/pulsar/pull/11346 ([merlimat](https://github.com/merlimat))

- [Admin] Fix the error that the batch size is smaller than `0` when peeking messages.

    https://github.com/apache/pulsar/pull/11301 ([aloyszhang](https://github.com/aloyszhang))

- [Broker] Fix the NPE that occurs when unloading persistent partitioned topics.

    https://github.com/apache/pulsar/pull/11310 ([wuzhanpeng](https://github.com/wuzhanpeng))

- [Policy] Fix the issue that names of partitioned topics are used to get topic-level policies.

    https://github.com/apache/pulsar/pull/11294 ([315157973](https://github.com/315157973))

- [Broker] Fix the issue of retention of keys in compaction.

    https://github.com/apache/pulsar/pull/11287 ([merlimat](https://github.com/merlimat))

### Event / News

- July Pulsar Monthly Update -- Exactly Once with Transactions

    - https://www.youtube.com/watch?v=VOcleimYlW0

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).