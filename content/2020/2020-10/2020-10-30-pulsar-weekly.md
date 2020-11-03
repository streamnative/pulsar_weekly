---
title: "2020-10-30-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-10-24 ~ 2020-10-30"
date: 2020-10-24 ~ 2020-10-30
description: "This is the Pulsar community weekly update for 2020-10-24 ~ 2020-10-30, with updates on Pulsar client, broker, transaction, and so on."
id: "2020-10-30-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-10-24 ~ 2020-10-30

This is the Pulsar community weekly update for 2020-10-24 ~ 2020-10-30, with updates on Pulsar client, broker, transaction, tiered storage, and so on.

### Pulsar Highlight

The Pulsar Java client supports both `AvroBased` and `UnAvroBased` schemas. For details, see [PR-8246](https://github.com/apache/pulsar/pull/8246).

Before this PR is merged, the Pulsar Java client only supports the `AvroBased` schema.

by [@hnail](https://github.com/hnail))

### Notable Feature

- [Websocket] Update produce request and acknowledgement for WebSocket.

    https://github.com/apache/pulsar/pull/8401 ([@MarvinCai](https://github.com/MarvinCai))

- [Broker] Add the `nettyMaxFrameSizeBytes` setting to the `standalone.conf` file.

    https://github.com/apache/pulsar/pull/8385 ([@massakam](https://github.com/massakam))
    
- [Java Client] Disable the batch receiving timer for Readers.

    https://github.com/apache/pulsar/pull/8381 ([@lhotari](https://github.com/lhotari))

- [Broker] Allow the tenant Admin to loo kup topics.

    https://github.com/apache/pulsar/pull/8353 ([@rdhabalia]https://github.com/rdhabalia)
    
- [Broker] Implement the `TransactionBuffer` Refactor.

    https://github.com/apache/pulsar/pull/8347 ([@gaoran10]https://github.com/gaoran10)

- [Go Functions] Add the `newOuputMessage` interface for Go Function.

    https://github.com/apache/pulsar/pull/8327 ([@wolfstudy](https://github.com/wolfstudy))

- [Java client] Support cancelling message and batch futures returned from the reader and consumer.

    https://github.com/apache/pulsar/pull/8326 ([@lhotari](https://github.com/lhotari))
    
- [Broker] Delete the transaction marker for topics.

    https://github.com/apache/pulsar/pull/8318 ([@congbobo184](https://github.com/congbobo184))
    
- [Java client] Support the `UnAvroBased` Schema.

    https://github.com/apache/pulsar/pull/8246 ([@hnail](https://github.com/hnail))
    
- [Broker] Supporting deleting associated ledgers before deleting cluster metadata.

    https://github.com/apache/pulsar/pull/8244 ([@BewareMyPower]https://github.com/BewareMyPower)
    
- [Broker] Add broker configurations to enforce producer to publish encrypted messages.

    https://github.com/apache/pulsar/pull/8055 ([@rdhabalia](https://github.com/rdhabalia))
    
- [Admin API] Support looking up for partitioned topics.

    https://github.com/apache/pulsar/pull/7605 ([@aloyszhang](https://github.com/aloyszhang))
    
- [Broker] Support configuring the maximum concurrent HTTP Web requests.

    https://github.com/apache/pulsar/pull/7250 ([@rdhabalia](https://github.com/rdhabalia))

### Notable Bug Fix

- [Broker] Fix the deadlock that occurred during topic ownership check.

    https://github.com/apache/pulsar/pull/8406 ([@massakam](https://github.com/massakam))

- [Java client] Fix the issue that newly-created consumers cannot be paused for subscribing topics.

    https://github.com/apache/pulsar/pull/8387 ([@aloyszhang](https://github.com/aloyszhang))

- [Admin API] Validate the retention policy.

    https://github.com/apache/pulsar/pull/8358 ([@lhotari](https://github.com/lhotari))

- [Go client] Fix the memory leak issue for in the Golang client.

    https://github.com/apache/pulsar/pull/8325 ([@bschofield](https://github.com/bschofield))

- [Broker] Make the field names in `OffloadPolicies` match with those in config file.

    https://github.com/apache/pulsar/pull/8310 ([@gaoran10]https://github.com/gaoran10)

- [Broker] Refresh ZooKeeper-data cache in background to avoid deadlock and blocking IO on ZK thread.

    https://github.com/apache/pulsar/pull/8304 ([@rdhabalia](https://github.com/rdhabalia))

- [Python client] Expose schema version (of writerSchema) in messages.

    https://github.com/apache/pulsar/pull/8173 ([@shiv4289](https://github.com/shiv4289))

- [Proxy] Fix the memory leak issue caused by the the debug log level.

    https://github.com/apache/pulsar/pull/7963 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Support using the Kubernetes runtime to customize the class path of the function instance.

    https://github.com/apache/pulsar/pull/7844 ([@nlu90](https://github.com/nlu90))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Traning]

  - Low-Latency Stream Processing with Jet

    Slides: https://www.slideshare.net/streamnative/low-latency-stream-processing-with-jet

    Video: https://www.youtube.com/watch?v=wIJGusBxB70

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

### Blog / Article

- StreamNative Announces Free Cloud Offering

  - https://streamnative.io/blog/release/2020-10-28-streamnative-free-cloud
