---
title: "2021-07-12-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-07-05 ~ 2021-07-11"
date: 2021-07-05 ~ 2021-07-11
description: "This is the Pulsar community weekly update for 2021-07-05 ~ 2021-07-11, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-07-12-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-07-05 ~ 2021-07-11

This is the Pulsar community weekly update for 2021-07-05 ~ 2021-07-11, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- PIP-45: Remove `localZkCache` access from `AdminResource`. All accesses go through the `MetadataStore`.

    https://github.com/apache/pulsar/pull/11265 ([@merlimat](https://github.com/merlimat))

- PIP-45: Change topic initialization to use `MetadataStore` and to be fully asynchronously.

    https://github.com/apache/pulsar/pull/11217 ([@merlimat](https://github.com/merlimat))

### Notable Feature

- [Policy] Support setting `Null` as the namespace-level subscription TTL.

    https://github.com/apache/pulsar/pull/11253 ([@massakam](https://github.com/massakam))

- [Pulsar Adapters] Add the link to the Apache Pulsar Adapter 2.8.0 to the **Download** page (only the source tarball).

    https://github.com/apache/pulsar/pull/11247 ([@eolivelli](https://github.com/eolivelli))

- [Admin] Enable peeking encrypted batch messages.
    
    https://github.com/apache/pulsar/pull/11244 ([@massakam](https://github.com/massakam))

- Add a usage example for the Redis sink.
    
    https://github.com/apache/pulsar/pull/11222 ([@murong00](https://github.com/murong00))

### Notable Bug Fix

- [Client] Fix the WebSocket TLS bug.

    https://github.com/apache/pulsar/pull/11243 ([@Technoboy-](https://github.com/Technoboy-))

- [Policy] Fix the issue that too many ledgers are deleted based on the retention size policy.

    https://github.com/apache/pulsar/pull/11242 ([@aloyszhang](https://github.com/aloyszhang))

- [Client] Fix the issue that the cluster data fails to be retrieved due to the empty `ConfigurationStoreServers`.
    
    https://github.com/apache/pulsar/pull/11234 ([@Technoboy-](https://github.com/Technoboy-))

- [Metrics] Fix some missing replicator metrics.

    https://github.com/apache/pulsar/pull/11264 ([@Technoboy-](https://github.com/Technoboy-))

- [Test] Fix the test for Branch 2.7.
    
    https://github.com/apache/pulsar/pull/11254 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Fix the broker dispatch byte rate limiter (Branch 2.7).
    
    https://github.com/apache/pulsar/pull/11249 ([@gaoran10](https://github.com/gaoran10))

- [Ledger] Fix the ledger roll-over scheduler task  (Branch 2.7).
  
    https://github.com/apache/pulsar/pull/11226 ([@gaoran10](https://github.com/gaoran10))

- [Build] Use `entryTimestamp` for expiry checking in `internalGetMessageIdByTimestamp`.
    
    https://github.com/apache/pulsar/pull/11220 ([@freeznet](https://github.com/freeznet))

### Event / News

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).