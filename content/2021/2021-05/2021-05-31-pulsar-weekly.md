---
title: "2021-05-31-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-05-24 ~ 2021-05-30"
date: 2021-05-24 ~ 2021-05-30
description: "This is the Pulsar community weekly update for 2021-05-24 ~ 2021-05-30, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-05-31-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-05-24 ~ 2021-05-30

This is the Pulsar community weekly update for 2021-05-24 ~ 2021-05-30, with updates on Pulsar client, broker, transactions, and so on.

### Development

- Refactor the try-lock code pattern.

    https://github.com/apache/pulsar/pull/10742 ([@fantapsody](https://github.com/fantapsody))

- [C++] Reduce the redundant `redeliverMessages` when the message listener is enabled.

    https://github.com/apache/pulsar/pull/10726 ([@saosir](https://github.com/saosir))

- [Transaction] Add the transaction Admin API `getPendingAckInternalStats`.

    https://github.com/apache/pulsar/pull/10725 ([@congbobo184](https://github.com/congbobo184))

- [Schema] Support using `AutoProduceBytesSchema` as the function output schema.

    https://github.com/apache/pulsar/pull/10716 ([@gaoran10](https://github.com/gaoran10))

- [Common] Fix the inconsistent behavior in `LongPairRangeSet`.

    https://github.com/apache/pulsar/pull/10713 ([@315157973](https://github.com/315157973))

- [C++] Add the C++ single file logger factory.

    https://github.com/apache/pulsar/pull/10712 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Transaction] Fix the `WriteFail` state of the ManagedLedger in the transaction log.

    https://github.com/apache/pulsar/pull/10711 ([@congbobo184](https://github.com/congbobo184))

- [Java Client] On multi-topic consumers, do not keep checking the partitioned metadata.

    https://github.com/apache/pulsar/pull/10708 ([@merlimat](https://github.com/merlimat))

- [Transaction] Add the transaction Admin APIs `getSlowTransactions` and `getSlowTransactionsByCoordinatorId`.

    https://github.com/apache/pulsar/pull/10701 ([@congbobo184](https://github.com/congbobo184))

- [Schema] In `AutoConsumeSchema.decode`, proxy the call to `decode(payload, schemaversion)` correctly to the wrapped Schema.

    https://github.com/apache/pulsar/pull/10700 ([@eolivelli](https://github.com/eolivelli))

- [Broker] Avoid making copies of internal maps when iterating the custom HASH map.

    https://github.com/apache/pulsar/pull/10691 ([@merlimat](https://github.com/merlimat))

- [Transaction] Add the transaction Admin API `getTransactionMetadata`.

    https://github.com/apache/pulsar/pull/10690 ([@congbobo184](https://github.com/congbobo184))

- [Pulsar Proxy] Adjust the location of `logger.debug`.

    https://github.com/apache/pulsar/pull/10684 ([@mantuliu](https://github.com/mantuliu))

- [Broker] Optimize `getTopicPolicies` to avoid throwing  an unnecessary exception.

    https://github.com/apache/pulsar/pull/10683 ([@michaeljmarshall](https://github.com/michaeljmarshall))

- [Transaction] Add the transaction Admin API `getCoordinatorInternalStats`.

    https://github.com/apache/pulsar/pull/10653 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Add the transaction Admin APIs `getTransactionBufferStatus` and `getPendingAckStatus`.

    https://github.com/apache/pulsar/pull/10650 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Add the transaction Admin API `getTransactionInPendingAckStats`.

    https://github.com/apache/pulsar/pull/10648 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Add the transaction Admin API `getTransactionInBufferStats`.

    https://github.com/apache/pulsar/pull/10642 ([@congbobo184](https://github.com/congbobo184))

- [Function] Add `--batch-source-config` switch to the Pulsar Admin source API.

    https://github.com/apache/pulsar/pull/10593 ([@david-streamlio](https://github.com/david-streamlio))

- [Broker] Migrate `NamespaceService` to use `MetadataStore`.

    https://github.com/apache/pulsar/pull/10532 ([@merlimat](https://github.com/merlimat))

### Notable Bug Fix

- [Function] Use the default Kubernetes secret mount permission to allow non-root user to read the authentication token.

    https://github.com/apache/pulsar/pull/10743 ([@zzzming](https://github.com/zzzming))

- [ManagedLedger] Fix the original solution which is used to prevent race conditions between timeout and completion.

    https://github.com/apache/pulsar/pull/10740 ([@lhotari](https://github.com/lhotari))

- [ManagedLedger] Fix the scheduled task cancellation operation to make it happen earlier in the `asyncClose` method.

    https://github.com/apache/pulsar/pull/10739 ([@lhotari](https://github.com/lhotari))

- [Java Client] Add error message to `setMaxPendingMessagesAcrossPartitions`.

    https://github.com/apache/pulsar/pull/10709 ([@wenbingshen](https://github.com/wenbingshen))

- [Broker] Asynchronize the method `onManagedLedgerLastLedgerInitialize` for `ManagedLedgerInterceptor`.

    https://github.com/apache/pulsar/pull/10706 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the NPE that occurs when filtering read entries.

    https://github.com/apache/pulsar/pull/10704 ([@315157973](https://github.com/315157973))

- [Broker] Fix the issue that `StackOverflowError` occurs when trying to redeliver a large number of acknowledged messages.

    https://github.com/apache/pulsar/pull/10696 ([@massakam](https://github.com/massakam))

- [Transaction] Fix the issue that the transaction acknowledges one topic with multiple subscriptions.

    https://github.com/apache/pulsar/pull/10689 ([@congbobo184](https://github.com/congbobo184))

- Fix binary license check issues and update Jersey to 2.34 for Pulsar SQL.

    https://github.com/apache/pulsar/pull/10682 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix issues in `advanceNonDurableCursors`.

    https://github.com/apache/pulsar/pull/10667 ([@jerrypeng](https://github.com/jerrypeng))

- [Broker] Catch the exception in `checkSubscriptionTypesEnable`.

    https://github.com/apache/pulsar/pull/10341 ([@hangc0276](https://github.com/hangc0276))

### Event / News

- Pulsar Virtual Summit North America 2021

    - Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

  - Intro to Apache Pulsar EP04

    - 05/27: https://www.youtube.com/watch?v=6qpx37dRBB0 

### Blog / Article

- Fast JMS for Apache Pulsar: Modernize and Reduce Costs with Blazing Performance -- Enrico Olivelli

    - https://www.datastax.com/blog/fast-jms-apache-pulsar?utm_source=thenewstack&utm_medium=twitter&utm_campaign=platform

- Monitoring the Health of Apache Pulsar with Pulsar Heartbeat -- Ming Luo

    - https://www.datastax.com/blog/monitoring-health-apache-pulsar-pulsar-heartbeat
