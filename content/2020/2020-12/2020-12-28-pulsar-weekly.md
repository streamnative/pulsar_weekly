---
title: "2020-12-28-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-12-19 ~ 2020-12-27"
date: 2020-12-19 ~ 2020-12-27
description: "This is the Pulsar community weekly update for 2020-12-19 ~ 2020-12-27, with updates on Pulsar client, broker, Functions, transactions, KoP, and so on."
id: "2020-12-28-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-12-19 ~ 2020-12-27

This is the Pulsar community weekly update for 2020-12-19 ~ 2020-12-27, with updates on Pulsar client, broker, Functions, transactions, KoP, and so on.

### Pulsar Highlight

Introduce the continuous offset for Pulsar. The continuous message sequence ID for messages in one topic-partition is useful for the protocol handler like KoP.

by [@aloyszhang](https://github.com/aloyszhang)

### Notable Feature

- [Functions] Adding timeout to open table call for the function state.

    https://github.com/apache/pulsar/pull/9006 ([@jerrypeng](https://github.com/jerrypeng))

- [Perf] Enable pulsar-perf to load WebSocket service URL from the configuration file.

    https://github.com/apache/pulsar/pull/9000 ([@massakam](https://github.com/massakam))

- [Functions] Allow stats operations not to be blocked in functions.

    https://github.com/apache/pulsar/pull/9005 ([@jerrypeng](https://github.com/jerrypeng))

- [Broker] Improve error handling when the broker does not trust client certificates.

    https://github.com/apache/pulsar/pull/8998 ([@sijie](https://github.com/sijie))

- [Broker] Make namespaces isolation policy updates take effect on time.

    https://github.com/apache/pulsar/pull/8976 ([@jiazhai](https://github.com/jiazhai))

- [Broker] Add the if-branch for `SubscriptionBusyException`.

    https://github.com/apache/pulsar/pull/9017 ([@cimura](https://github.com/cimura))

- [Broker] Remove the duplicated broker prometheus metrics type.

    https://github.com/apache/pulsar/pull/8995 ([@zzzming](https://github.com/zzzming))

- [Broker] Add the raw prometheus metrics provider.

    https://github.com/apache/pulsar/pull/9021 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Perform automatic certification refresh for pulsar-admin.

    https://github.com/apache/pulsar/pull/8831a ([@rdhabalia](https://github.com/rdhabalia))

- [SQL] Add retry for the SQL test.

    https://github.com/apache/pulsar/pull/9010 ([@zymap](https://github.com/zymap))

- [C++] Correct the argument name of the subscribe API.

    https://github.com/apache/pulsar/pull/9037 ([@saosir](https://github.com/saosir))

- [Broker] Introduce the continuous offset for pulsar.

    https://github.com/apache/pulsar/pull/9039 ([@aloyszhang](https://github.com/aloyszhang))

- [WebSocket] Return the status code depending on type of `PulsarClientException`.

    https://github.com/apache/pulsar/pull/9031 ([@massakam](https://github.com/massakam))

- [Broker] Add the `updateRates` method for KoP to collect the publishing rate.

    https://github.com/apache/pulsar/pull/9049 ([@dockerzhang](https://github.com/apache/pulsar/pull/9049))

- [Broker] Make the Netty Acceptor ThreadPool size configurable.

    https://github.com/apache/pulsar/pull/9061 ([@Shoothzj](https://github.com/Shoothzj))

- [Broker] Support peeking broker entry metadata.

    https://github.com/apache/pulsar/pull/9067 ([@aloyszhang](https://github.com/aloyszhang))

### Notable Bug Fix

- [Common] Fix the issue that peeking compressed messages throws an exception (Readonly buffers are not supported by Airlift.).

    https://github.com/apache/pulsar/pull/8990 ([@eolivelli](https://github.com/eolivelli))

- [Transaction] Fix the transaction messages order error and the deduplication error.

    https://github.com/apache/pulsar/pull/9024 ([@gaoran10](https://github.com/gaoran10))

- [Broker] Fix the issue that `DelayedDelivery` at the broker level has a default value.

    https://github.com/apache/pulsar/pull/9030 ([@315157973](https://github.com/315157973))

- [pulsar-managed-ledger-admin] Support deleting multiple Ledgers.

    https://github.com/apache/pulsar/pull/9009 ([@milos-matijasevic](https://github.com/milos-matijasevic))

- [Client] Fix the unavailable hash range condition.

    https://github.com/apache/pulsar/pull/9041 ([@k2la](https://github.com/k2la))

- [Proxy] Ensure to return correct Authz and authentication errors from Pulsar proxy to client.

    https://github.com/apache/pulsar/pull/9055 ([@jerrypeng](https://github.com/jerrypeng))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq

### Blog / Article

- What's New in Apache Pulsar 2.7.0

    - https://streamnative.io/en/blog/release/2020-12-25-pulsar-270

- What's New in Pulsar Flink Connector 2.7.0

    - https://streamnative.io/en/blog/release/2020-12-24-pulsar-flink-connector-270