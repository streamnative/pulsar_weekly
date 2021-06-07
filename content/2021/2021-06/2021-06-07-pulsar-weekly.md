---
title: "2021-06-07-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-05-31 ~ 2021-06-06"
date: 2021-05-31 ~ 2021-06-06
description: "This is the Pulsar community weekly update for 2021-05-31 ~ 2021-06-06, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-06-07-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-05-31 ~ 2021-06-06

This is the Pulsar community weekly update for 2021-05-31 ~ 2021-06-06, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Sink] Support using Kafka's sinks as Pulsar's sinks.

    https://github.com/apache/pulsar/pull/9927 ([@dlg99](https://github.com/dlg99))

### Notable Feature

- [Metrics] Use the ZooKeeper Prometheus metric provider to export ZooKeeper metrics.

    https://github.com/apache/pulsar/pull/10803 ([@hangc0276](https://github.com/hangc0276))

- [Transaction] Add `managedLedger` metrics to Prometheus metrics.

    https://github.com/apache/pulsar/pull/10761 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Add the advertised `listenerName` for the geo-replicator to connect to a remote cluster.

    https://github.com/apache/pulsar/pull/10751 ([@wangjialing218](https://github.com/wangjialing218))
    
- [Transaction] Add the synchronization method for the transaction Admin API.

    https://github.com/apache/pulsar/pull/10745 ([@congbobo184](https://github.com/congbobo184))

- [BookKeeper] Upgrade BookKeeper to version 4.14.1.

    https://github.com/apache/pulsar/pull/10686 ([@hangc0276](https://github.com/hangc0276))

### Notable Bug Fix

- [Pulsar SQL] Fix Pulsar SQL issues that occur when running `select count(*)` for the table with the primary schema.

    https://github.com/apache/pulsar/pull/10840 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the issue that the consumer is stuck due to reuse of the entry wrapper.

  https://github.com/apache/pulsar/pull/10824 ([@codelipenghui](https://github.com/codelipenghui))
  
- [Schema] Fix the NEP that occurs when `AutoConsumeSchema` decodes messages with a null schema version.

  https://github.com/apache/pulsar/pull/10811 ([@gaoran10](https://github.com/gaoran10))
  
- [Build] Support building the Pulsar website without setting the `CROWDIN_DOCUSAURUS_API_KEY`.

  https://github.com/apache/pulsar/pull/10804 ([@lhotari](https://github.com/lhotari))
  
- [Kinesis] Fix the issue that the Kinesis sink connector does not acknowledge messages.

    https://github.com/apache/pulsar/pull/10769 ([@RobertIndie](https://github.com/RobertIndie))

- [Java Client]Unlock the write lock of the `UnAckedMessageTracker` before calling `redeliverUnacknowledgedMessages`.

    https://github.com/apache/pulsar/pull/10768 ([@codelipenghui](https://github.com/codelipenghui))

- [BookKeeper] Add a read lock when traversing `batchDeletedIndexes`.

    https://github.com/apache/pulsar/pull/10763 ([@315157973](https://github.com/315157973))

- [Transaction] Fix the path pass parameter issue for the transaction Admin API.

    https://github.com/apache/pulsar/pull/10748 ([@congbobo184](https://github.com/congbobo184))
    
- [Broker] Enable updating `ManagedLedgerConf#maximumRolloverTimeMs`.

    https://github.com/apache/pulsar/pull/10746 ([@wuzhanpeng](https://github.com/wuzhanpeng))

- [Kinesis] Fix the issue that the Kinesis sink `Backoff` class is not found.

    https://github.com/apache/pulsar/pull/10744 ([@gaoran10](https://github.com/gaoran10))

- [Schema] Fix the issue that the dead letter producer does not handle `AUTO_CONSUME_SCHEMA`.

    https://github.com/apache/pulsar/pull/9970 ([@congbobo184](https://github.com/congbobo184))

### Event / News

- Pulsar Virtual Summit North America 2021

    - Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Pulsar Isolation for Dummies: Separate Pulsar Clusters

    - https://streamnative.io/en/blog/tech/2021-06-03-pulsar-isolation-for-dummies-separate-pulsar-clusters

- Building Connectors On Pulsar Made Simple

    - https://streamnative.io/en/blog/tech/2021-06-01-building-connectors-on-pulsar-made-simple