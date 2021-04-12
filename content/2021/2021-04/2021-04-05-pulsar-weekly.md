---
title: "2021-04-05-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-03-29 ~ 2021-04-04"
date: 2021-03-29 ~ 2021-04-04
description: "This is the Pulsar community weekly update for 2021-03-29 ~ 2021-04-04, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-04-05-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-03-29 ~ 2021-04-04

This is the Pulsar community weekly update for 2021-03-29 ~ 2021-04-04, with updates on Pulsar client, broker, transactions, and so on.

### Development

- [Broker] Fix the `NonDurableCursorImpl#initialPosition` issue that is caused when the `startMessageId` is greater than `lastConfirmedEntry`.

    https://github.com/apache/pulsar/pull/10095 ([@congbobo184](https://github.com/congbobo184))

- [C++ client] Reduce the level of the `ack-grouping` tracker logs.

    https://github.com/apache/pulsar/pull/10094 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Broker] Fix `KeyValue` encoding issue of `AutoConsumeSchema`.

    https://github.com/apache/pulsar/pull/10089 ([@vroyer](https://github.com/vroyer))

- [Broker] Optimize `CompletableFuture` timeout handling.

    https://github.com/apache/pulsar/pull/10065 ([@lhotari](https://github.com/lhotari))

- [Broker] Change the level of the `police cache not init` logs.

    https://github.com/apache/pulsar/pull/10059 ([@hangc0276](https://github.com/hangc0276))

- [Tiered Storage] Restore Offloader directory Overriding to prevent Class Loader Leak.

    https://github.com/apache/pulsar/pull/9878 ([@michaeljmarshall](https://github.com/michaeljmarshall))

### Notable Feature

- [Broker] Add the new `Optional<Object> Schema#getNativeSchema` method.

    https://github.com/apache/pulsar/pull/10076 ([@eolivelli](https://github.com/eolivelli))

### Notable Bug Fix

- [Broker] Fix the issue that the `MaxConsumersPerSubscriptionn` can not be disabled and removed.

    https://github.com/apache/pulsar/pull/10070 ([@315157973](https://github.com/315157973))

- [Client] Use a common request timeout handling for lookup requests to fix the possible memory leak.

    https://github.com/apache/pulsar/pull/10066 ([@lhotari](https://github.com/lhotari))

- [Client] Remove unnecessary locks from `ConsumerImpl`.

    https://github.com/apache/pulsar/pull/9261 ([@hangc0276](https://github.com/hangc0276))

- [Client] Fix the bug that the `brokerTimestamp` is set improperly.

    https://github.com/apache/pulsar/pull/9493 ([@hangc0276](https://github.com/hangc0276))

- [Client] Allow Pulsar client to receive the external timer.

    https://github.com/apache/pulsar/pull/9802 ([@linlinnn](https://github.com/linlinnn))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- Apache Pulsar Hackathon

    Sign-up: https://www.eventbrite.com/e/apache-pulsar-hackathon-2021-tickets-143906003731

- Pulsar Virtual Summit North America 2021

    Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021