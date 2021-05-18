---
title: "2021-05-17-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-05-10 ~ 2021-05-16"
date: 2021-05-10 ~ 2021-05-16
description: "This is the Pulsar community weekly update for 2021-05-10 ~ 2021-05-16, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-05-17-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-05-10 ~ 2021-05-16

This is the Pulsar community weekly update for 2021-05-10 ~ 2021-05-16, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Transaction] Handle transaction pending ack persistence.
  
  https://github.com/apache/pulsar/pull/8881 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Migrate the schema storage metadata to `MetadataStore`.
  
  https://github.com/apache/pulsar/pull/10545 ([@merlimat](https://github.com/merlimat))

- [Docker] Add a new docker compose that includes all the Pulsar components.
  
  https://github.com/apache/pulsar/pull/10409 ([@odmarkj](https://github.com/odmarkj))

### Development

- [PIP-85] Add the schema information to messages in the Java Client API.
  
  https://github.com/apache/pulsar/pull/10476 ([@eolivelli](https://github.com/eolivelli))

### Notable Feature

- [Python Client] Replace `Exceptions` with `PulsarExceptions`.
  
  https://github.com/apache/pulsar/pull/7600 ([@lbenc135](https://github.com/lbenc135))

- [Enhancement] The reader supports seeking messages from the separate message ID or time.
  
  https://github.com/apache/pulsar/pull/10348 ([@315157973](https://github.com/315157973))

- [CLI] Support setting the time-based limit on the backlog quota through CLI.
  
  https://github.com/apache/pulsar/pull/10401 ([@MarvinCai](https://github.com/MarvinCai))

- [Pulsar IO] Use `Message.getReaderSchema()` in Pulsar sink connectors when possible.
  
  https://github.com/apache/pulsar/pull/10557 ([@eolivelli](https://github.com/eolivelli))

- [Broker] Expose the topic-level `averageMsgSize` to metrics.
  
  https://github.com/apache/pulsar/pull/10553 ([@315157973](https://github.com/315157973))

- [Enhancement] Support truncating all data of a topic without disconnecting the producers and consumers.
  
  https://github.com/apache/pulsar/pull/10326 ([@jangwind](https://github.com/jangwind))

- [Enhancement] Support creating `MetadataCache` with the custom SerDe.
  
  https://github.com/apache/pulsar/pull/10543 ([@merlimat](https://github.com/merlimat))

- [Broker] Get durable subscription without handling `startMessageRollbackDurationSec`.
  
  https://github.com/apache/pulsar/pull/10520 ([@linlinnn](https://github.com/linlinnn))

- [Auth] Enable Conscrypt for Jetty in the Pulsar broker and in the Pulsar proxy.
  
  https://github.com/apache/pulsar/pull/10541 ([@lhotari](https://github.com/lhotari))

- [Broker] Dispatch messages to consumers with permits.
  
  https://github.com/apache/pulsar/pull/10417 ([@rdhabalia](https://github.com/rdhabalia))

- [Enhancement] Support disabling the maximum queue size for the producers.
  
  https://github.com/apache/pulsar/pull/9650 ([@merlimat](https://github.com/merlimat))

- [Auth] Support the optional authentication method name header in HTTP authentication.
  
  https://github.com/apache/pulsar/pull/6799 ([@KannarFr](https://github.com/KannarFr))

### Notable Bug Fix

- [Broker] Fix the issue that the `AdvertisedAddress` in `PusarService` and in `conf.` is inconsistent.
  
  https://github.com/apache/pulsar/pull/10312 ([@315157973](https://github.com/315157973))

- [Client] Fix the NPE that is thrown when an ACK grouping tracker checks duplicated message IDs.
  
  https://github.com/apache/pulsar/pull/10586 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Test] Fix the `GracefulExecutorServicesShutdownTest` flaky test.
  
  https://github.com/apache/pulsar/pull/10599 ([@lhotari](https://github.com/lhotari))

- [Function] Fix the sink or source exception stats.
  
  https://github.com/apache/pulsar/pull/10549 ([@linlinnn](https://github.com/linlinnn))

- [Client] Fix the default retry letter and the dead letter topic name.
  
  https://github.com/apache/pulsar/pull/10129 ([@wangjialing218](https://github.com/wangjialing218))

- [Broker] Fix the bug that occurs when checking whether a partitioned topic is a system topic.
  
  https://github.com/apache/pulsar/pull/10529 ([@hangc0276](https://github.com/hangc0276))

- [Broker] Make `OpAddEntry.toString()` more robust to nulls to prevent NPEs.
  
  https://github.com/apache/pulsar/pull/10548 ([@devinbost](https://github.com/devinbost))

- [Transaction] Fix the transaction buffer delete marker issue.
  
  https://github.com/apache/pulsar/pull/10525 ([@congbobo184](https://github.com/congbobo184))

- [Test] Refactor the function integration tests for easier maintainability.
  
  https://github.com/apache/pulsar/pull/10140 ([@david-streamlio](https://github.com/david-streamlio))

### Event / News

- Pulsar Virtual Summit North America 2021

    - Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - 022: May Project Updates on Apache Pulsar

      - https://www.youtube.com/watch?v=4RJXJBB_1UU

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Apache Pulsar — Development Setup -- alpha2phi

    - https://alpha2phi.medium.com/apache-pulsar-development-setup-bbdc82314cf

- 7 Reasons to Choose Apache Pulsar over Apache Kafka -- Chris Bartholomew

    - https://datastax.medium.com/7-reasons-to-choose-apache-pulsar-over-apache-kafka-cb111087eadb

- Pulsar Virtual Summit North America 2021: Speakers Announced

    - https://streamnative.io/en/blog/community/2021-05-12-pulsar-virtual-summit-north-america-2021-speakers-announced