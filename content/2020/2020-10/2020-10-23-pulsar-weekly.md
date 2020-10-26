---
title: "2020-10-23-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-10-17 ~ 2020-10-23"
date: 2020-10-17 ~ 2020-10-23
description: "This is the Pulsar community weekly update for 2020-10-17 ~ 2020-10-23, with updates on Pulsar client, broker, Pulsar Functions, transaction, tiered storage, and so on."
id: "2020-10-23-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-10-17 ~ 2020-10-23

This is the Pulsar community weekly update for 2020-10-17 ~ 2020-10-23, with updates on Pulsar client, broker, Pulsar Functions, transaction, tiered storage, and so on.

### Pulsar Highlight

Pulsar has supported acknowledging the batch message index since release 2.6.0. But Pulsar does not support setting the cursor. If users reset the cursor to a batch index of the batch message when consuming messages again, they will get the batch index again. Now, Pulsar supports resetting the cursor to a batch index of the batch message.

by [@Renkai](https://github.com/Renkai)

### Notable Feature

- [Tiered Storage] Refactor JCloud tiered storage to support additional JClouds-supported providers.

    https://github.com/apache/pulsar/pull/6335 ([@david-streamlio](https://github.com/david-streamlio))

- [Metrics] Add metrics for topic lookups operations.

    https://github.com/apache/pulsar/pull/8272 ([@merlimat](https://github.com/merlimat))

- [Pulsar Functions] Organize and enhance the example directory in Go functions.

    https://github.com/apache/pulsar/pull/8288 ([@wolfstudy](https://github.com/wolfstudy))

- [Transaction] Adjust the interface `TransactionBuffer`.

    https://github.com/apache/pulsar/pull/8291 ([@gaoran10](https://github.com/gaoran10))

- [Pulsar Broker] Add the REST handler to determine whether the broker is fully ready to accept requests.

    https://github.com/apache/pulsar/pull/8303 ([@merlimat](https://github.com/merlimat))

- [Pulsar Broker] Close ZooKeeper connections at end of metadata setup.

    https://github.com/apache/pulsar/pull/8228 ([@bmyers-csu](https://github.com/bmyers-csu))

- [Pulsar Broker] Support limiting the maximum subscriptions per topic.

    https://github.com/apache/pulsar/pull/8289 ([@hangc0276](https://github.com/hangc0276))

- [Pulsar Bookie] Refine the BookKeeper metadata service URI when initializing the metadata.

    https://github.com/apache/pulsar/pull/8269 ([@murong00](https://github.com/murong00))

- [Pulsar Functions] Add access to the current message from the function context.

    https://github.com/apache/pulsar/pull/8290 ([@vaihtovirta](https://github.com/vaihtovirta))

- [Pulsar Broker] Support resetting the cursor to a batch index of the batching message.

    https://github.com/apache/pulsar/pull/8285 ([@Renkai](https://github.com/Renkai))

- [Pulsar Broker] Support excluding the message when resetting the cursor based on the message ID.

    https://github.com/apache/pulsar/pull/8306 ([@315157973](https://github.com/315157973))

- [Pulsar Broker] Support replication dispatch-rate limiting for namespace API (V1).

    https://github.com/apache/pulsar/pull/8314 ([@rdhabalia](https://github.com/rdhabalia))

- [Pulsar Admin] Support resetting the cursor to a batch index for the Pulsar Admin.

    https://github.com/apache/pulsar/pull/8329 ([@codelipenghui](https://github.com/codelipenghui))

- [Pulsar Broker] Configure the namespace anti-affinity policy in local policies.

    https://github.com/apache/pulsar/pull/8349 ([@rdhabalia](https://github.com/rdhabalia))

- [Pulsar Proxy] Add the Proxy plugin interface to support the additional user-defined servlet.

    https://github.com/apache/pulsar/pull/8067 ([@wolfstudy](https://github.com/wolfstudy))

### Notable Bug Fix

- [Managed Ledger] Fix the issue that the broker enters an infinite loop in `ManagedLedgerImpl.asyncReadEntries`.

    https://github.com/apache/pulsar/pull/8284 ([@hangc0276](https://github.com/hangc0276))

- [C++ Client] Fix the issue that the client always allocates more buffers than required.

    https://github.com/apache/pulsar/pull/8283 ([@merlimat](https://github.com/merlimat))

- [Pulsar Standalone] Fix the issue that when running ZooKeeper in standalone mode, old snapshots are not deleted.

    https://github.com/apache/pulsar/pull/8217 ([@merlimat](https://github.com/merlimat))

- [Managed Ledger] Fix the race condition in updating `readPosition` in `ManagedCursorImpl`.

    https://github.com/apache/pulsar/pull/8299 ([@lhotari](https://github.com/lhotari))

- [Pulsar Broker] Fix the message TTL and the ordering issue for replaying messages in the Key_Shared subscription mode.

    https://github.com/apache/pulsar/pull/8292 ([@codelipenghui](https://github.com/codelipenghui))

- [Pulsar Broker] Use `cacheExpirySeconds` configuration for the expire time of the ZooKeeper cache.

    https://github.com/apache/pulsar/pull/8302 ([@rdhabalia](https://github.com/rdhabalia))

- [C++ Client] Fix the segfault in unit test due to uninitialized member variables.

    https://github.com/apache/pulsar/pull/8334 ([@merlimat](https://github.com/merlimat))

- [C++ Client] Fix the issue that back-pressure is implemented on batches rather than number of messages.

    https://github.com/apache/pulsar/pull/8331 ([@merlimat](https://github.com/merlimat))

- [Pulsar Broker] Fix the issue that the split-bundle API overwrites `LocalPolicies`.

    https://github.com/apache/pulsar/pull/8313 ([@rdhabalia](https://github.com/rdhabalia))

- [C++ Client] Fix the message ID error when subscribing to a single partition.

    https://github.com/apache/pulsar/pull/8341 ([@BewareMyPower](https://github.com/BewareMyPower))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

  - Low-Latency Stream Processing with Jet

    https://us02web.zoom.us/webinar/register/3216003857537/WN_821OFj6ITN23Y8uf8KgEag

### Blog / Article

- Introducing Cloud Storage Sink Connector - Streaming Data From Apache Pulsar to Cloud Objects

  - https://streamnative.io/blog/tech/2020-10-20-cloud-storage-sink-connector-251
