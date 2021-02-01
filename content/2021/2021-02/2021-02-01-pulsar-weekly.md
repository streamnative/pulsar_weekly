---
title: "2021-02-01-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-01-25 ~ 2021-01-31"
date: 2021-01-25 ~ 2021-01-31
description: "This is the Pulsar community weekly update for 2021-01-25 ~ 2021-01-31, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-02-01-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-01-25 ~ 2021-01-31

This is the Pulsar community weekly update for 2021-01-25 ~ 2021-01-31, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Pulsar Highlight

PIP-76: Streaming Offload separates data offloading from ledger rollover and offload the cached data as much as possible based on PIP-17. In addition, it provides a flexible user-perspective approach to control the data offloading behavior.

by ([@Renkai](https://github.com/Renkai))

### Development

- [Broker] Add a command to refresh authentication data in the Pulsar broker.

    https://github.com/apache/pulsar/pull/9064 ([@zymap](https://github.com/zymap))

- [Transactions] Implement transactions timeout.

    https://github.com/apache/pulsar/pull/9229 ([@congbobo184](https://github.com/congbobo184))

- [Security] Add authentication metrics.

    https://github.com/apache/pulsar/pull/9244 ([@RobertIndie](https://github.com/RobertIndie))

- [Admin] Lazily initialize `PulsarAdmin` in `PulsarAdminTool`.

    https://github.com/apache/pulsar/pull/9312 ([@eolivelli](https://github.com/eolivelli))

- [Client] Support the JSON-format token.

    https://github.com/apache/pulsar/pull/9313 ([@RobertIndie](https://github.com/RobertIndie))

### Notable Feature

- [Broker] Support getting the applied policy for `MaxProducer`.

    https://github.com/apache/pulsar/pull/9293 ([@315157973](https://github.com/315157973))

- [Broker] Broker resources use metadata-store API.

    https://github.com/apache/pulsar/pull/9346 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Cluster resources use metadata-store API.

    https://github.com/apache/pulsar/pull/9338 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Support fetching the metadata from the entry data in the `publish` callback.

    https://github.com/apache/pulsar/pull/9257 ([@BewareMyPower](https://github.com/BewareMyPower))

### Notable Bug Fix

- [Broker] Fix the issue with not skipping the broker's entry metadata when peeking the message metadata.

    https://github.com/apache/pulsar/pull/9255 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the issue with failing to automatically creating the system topic.

    https://github.com/apache/pulsar/pull/9272 ([@315157973](https://github.com/315157973))

- [Python] Return the `MessageId` in producer's synchronous `send` method.

    https://github.com/apache/pulsar/pull/9287 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Tiered Storage] Fix the fake `complete` issue in offloading.

    https://github.com/apache/pulsar/pull/9306 ([@Renkai](https://github.com/Renkai))

### Ecosystem

- [Broker] Make the BookKeeper shell more user-friendly.

    https://github.com/apache/pulsar/pull/9281 ([@eolivelli](https://github.com/eolivelli))

- [Function] Add the metrics server to Go Function.

    https://github.com/apache/pulsar/pull/9318 ([@freeznet](https://github.com/))

### Event / News

- [Webinar] Watch Your Streams: Implementing OpenTelemetry with Apache Pulsar

    - Video: https://www.youtube.com/channel/UCywxUI5HlIyc0VEKYR4X9Pg/featured

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

### Blog / Article

- Making the Most of the Apache Pulsar Messaging Platform Has Never Been Easier --  Callie Wallace

    - https://www.tibco.com/blog/2021/01/28/making-the-most-of-the-apache-pulsar-messaging-platform-has-never-been-easier/