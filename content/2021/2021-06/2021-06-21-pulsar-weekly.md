---
title: "2021-06-21-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-06-14 ~ 2021-06-20"
date: 2021-06-14 ~ 2021-06-20
description: "This is the Pulsar community weekly update for 2021-06-14 ~ 2021-06-20, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-06-21-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-06-14 ~ 2021-06-20

This is the Pulsar community weekly update for 2021-06-14 ~ 2021-06-20, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Broker] Stop the replicator for failed and timed-out topics and clean up failed topics.

    https://github.com/apache/pulsar/pull/10847 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] When the Replicator is enabled, no managedLedger is created when updating the number of partitions.

    https://github.com/apache/pulsar/pull/10910 ([@315157973](https://github.com/315157973))

### Notable Feature

- [Security] Exclude and remove the [FreeBuilder](https://github.com/inferred/FreeBuilder) dependency.

    https://github.com/apache/pulsar/pull/10869 ([@lhotari](https://github.com/lhotari))

- [Security] Upgrade BouncyCastle to version 1.69.

    https://github.com/apache/pulsar/pull/10867 ([@lhotari](https://github.com/lhotari))

- [Security] Upgrade the Kubernetes Java client to version 12.0.1.

    https://github.com/apache/pulsar/pull/10866 ([@lhotari](https://github.com/lhotari))

- [Security] Upgrade Caffeine to version 2.9.1.

    https://github.com/apache/pulsar/pull/10865 ([@lhotari](https://github.com/lhotari))

- [Python] Add Python 3.9 to `manylinux2014` build support.

    https://github.com/apache/pulsar/pull/10954 ([@lbenc135](https://github.com/lbenc135))

- [Broker] Remove the redundant method for `CompletableFuture` timeout handling.

    https://github.com/apache/pulsar/pull/10970 ([@lhotari](https://github.com/lhotari))

- [Test] Add some tests for `NamespaceBundleSplitAlgorithmTest`.

    https://github.com/apache/pulsar/pull/10987 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker] Stop the replicator for failed and timed-out topics and clean up failed topics.

    https://github.com/apache/pulsar/pull/10847 ([@rdhabalia](https://github.com/rdhabalia))

- [Refactor] Refactor some methods to Java 8.

    https://github.com/apache/pulsar/pull/10879 ([@mattisonchao](https://github.com/mattisonchao))

- [Test] Make Metadata `ZKSessionTest` less Flaky.

    https://github.com/apache/pulsar/pull/10955 ([@eolivelli](https://github.com/eolivelli))

- [Broker] When the Replicator is enabled, no managedLedger is created when updating the number of partitions.

    https://github.com/apache/pulsar/pull/10910 ([@315157973](https://github.com/315157973))

### Notable Bug Fix

- [Broker] Fix the direct memory leak in `getLastMessageId`.

    https://github.com/apache/pulsar/pull/10977 ([@lhotari](https://github.com/lhotari))

- [Broker] Fix `NonRecoverableLedgerException` when getting the last message ID by Reader.

    https://github.com/apache/pulsar/pull/10957 ([@codelipenghui](https://github.com/codelipenghui))

- [Build] Upgrade `io.airlift.aircompressor` to version 19.

    https://github.com/apache/pulsar/pull/10983 ([@newur](https://github.com/newur))

- [Common] Update the `TopicName#getPartitionIndex` implementation logic. 

    https://github.com/apache/pulsar/pull/10902 ([@yangl](https://github.com/yangl))

- [Proxy] Fix the string concatation in the loop.

    https://github.com/apache/pulsar/pull/10986 ([@mattisonchao](https://github.com/mattisonchao))

- [Metadata] Remove the duplicate `awaitility` dependency. 

    https://github.com/apache/pulsar/pull/10979 ([@yangl](https://github.com/yangl))

- [CLI] Fix the incorrect use of the `list.remove` method.

    https://github.com/apache/pulsar/pull/10935 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker] Fix the `parseMessageMetadata` error caused by not skipping the broker entry metadata.

    https://github.com/apache/pulsar/pull/10968 ([@aloyszhang](https://github.com/aloyszhang))

- [Client] Fix the issue that no return is available in `ConsumerImpl#internalGetLastMessageIdAsync`.

    https://github.com/apache/pulsar/pull/10974 ([@eolivelli](https://github.com/eolivelli))

- [C++] Fix the windows build issues about the static library.

    https://github.com/apache/pulsar/pull/10956 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Client] Fix the issue that non-persistent topics get partitioned metadata on discovery.

    https://github.com/apache/pulsar/pull/10806 ([@aloyszhang](https://github.com/aloyszhang))

- [Build] Fix the issue about the default `main` profile activation for Pulsar Functions.

    https://github.com/apache/pulsar/pull/10887 ([@murong00](https://github.com/murong00))

- [Transactions] Prevent the NPE that occurs when calling `closeAsync()` without a successful execution of `startAsync()`.

    https://github.com/apache/pulsar/pull/10948 ([@eolivelli](https://github.com/eolivelli))

- [Broker] Fix the issue that compaction does not work for the system topic.

    https://github.com/apache/pulsar/pull/10941 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the issue that some throwable exceptions are not thrown.

    https://github.com/apache/pulsar/pull/10931 ([@mattisonchao](https://github.com/mattisonchao))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Introducing StreamNative Platform

    - https://streamnative.io/en/blog/release/2021-06-16-streamnative-platform

- A Deep-dive of Transactions in Apache Pulsar

    - https://streamnative.io/en/blog/tech/2021-06-16-a-deep-dive-of-transactions-in-apache-pulsar

- Apache Pulsar Launches 2.8: Unified Messaging and Streaming With Transactions

    - https://streamnative.io/en/blog/release/2021-06-15-apache-pulsar-launches-2-8-unified-messaging-and-streaming-with-transactions

- Pulsar Hits Its 400th Contributor & Passes Kafka in Monthly Active Contributors

    - https://streamnative.io/en/blog/community/2021-06-14-pulsar-hits-its-400th-contributor-and-passes-kafka-in-monthly-active-contributors

- Exactly-Once Semantics with Transactions in Pulsar

    - https://streamnative.io/en/blog/release/2021-06-14-exactly-once-semantics-with-transactions-in-pulsar

- Why developers should use Apache Pulsar -- Patrick McFadin

    - https://www.infoworld.com/article/3619272/why-developers-should-use-apache-pulsar.html#tk.rss_all

- StreamNative Platform, An Enterprise Messaging and Streaming Platform Powered by Apache Pulsar

    - https://www.pressrelease.cc/2021/06/17/streamnative-platform-an-enterprise-messaging-and-streaming-platform-powered-by-apache-pulsar/