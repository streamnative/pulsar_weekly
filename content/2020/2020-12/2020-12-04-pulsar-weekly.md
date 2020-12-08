---
title: "2020-12-04-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-11-28 ~ 2020-12-04"
date: 2020-11-28 ~ 2020-12-04
description: "This is the Pulsar community weekly update for 2020-11-28 ~ 2020-12-04, with updates on Pulsar client, broker, Functions, tiered storage, and so on."
id: "2020-12-04-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-11-28 ~ 2020-12-04

This is the Pulsar community weekly update for 2020-11-28 ~ 2020-12-04, with updates on Pulsar client, broker, Functions, tiered storage, and so on.

### Pulsar Highlight

- [Functions] Support the key-based batch builder for Go Functions.
https://github.com/apache/pulsar/pull/8761 (@[wolfstudy](https://github.com/wolfstudy))

### Notable Feature

[Package management] Add package management service into the Pulsar startup process.
- https://github.com/apache/pulsar/pull/8764 (@[zymap](https://github.com/zymap))

[Functions] Support the key-based batch builder for Go Functions
- https://github.com/apache/pulsar/pull/8761 (@[wolfstudy](https://github.com/wolfstudy))

[C++] Optimize the batch message buffer allocation.
- https://github.com/apache/pulsar/pull/8749 (@[erobot](https://github.com/erobot))

[Package management] Support BookKeeper storage for packages management service.
- https://github.com/apache/pulsar/pull/8744 (@[zymap](https://github.com/zymap))

[Tiered storage] Support initializing the offload manager only once when creating the ledger offloader.
- https://github.com/apache/pulsar/pull/8739 (@[gaoran10](https://github.com/gaoran10))

### Notable Bug Fix

[Broker] Remove non-persistent subscription of topics from different threads to avoid deadlock when removing inactive subscriptions.
- https://github.com/apache/pulsar/pull/8820 (@[mkozioro](https://github.com/mkozioro))

[Broker] Support deleting all topics of a namespace when deleting a given namespace.
- https://github.com/apache/pulsar/pull/8806 (@[wangjialing218](https://github.com/wangjialing218))

[Function] Fix the single-quotes added to the user configuration.
- https://github.com/apache/pulsar/pull/8780 (@[wolfstudy](https://github.com/wolfstudy))

[Function] Fix the panic on discarded messages for Go Functions.
- https://github.com/apache/pulsar/pull/8776 (@[wolfstudy](https://github.com/wolfstudy))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq

### Blog / Article

- Impact of Apache Pulsar 2.7 release on the development of Infinitic -- Gilles Barbier

  - https://infinitic.substack.com/p/infinitic-updates-3

- Cloud-Native Apache Pulsar 2.7 Supports Transactions and Azure Blob Storage Offloader

  - https://streamnative.io/en/blog/release/2020-12-03-pulsar-270

- Work-Bench Snapshot: Augmenting Streaming and Batch Processing Workflows -- Priyanka Somrah 

  - https://medium.com/work-bench/work-bench-snapshot-augmenting-streaming-and-batch-processing-workflows-416e64d37a28

- How Apache Pulsar is Helping Iterable Scale its Customer Engagement Platform -- Greg Methvin

  - https://www.infoq.com/articles/pulsar-customer-engagement-platform/
