---
title: "2020-02-14-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-02-01 ~ 2020-02-14"
date: 2020-02-01 ~ 2020-02-14
description: "This is the Pulsar community weekly update for 2020-02-01 ~ 2020-02-14, with updates on refreshing authentication credentials, namespace level offloader, new bundle split algorithm to support evenly distributing topics, and many bug fixes and enhancements around helm chart."
---

## [Pulsar Community Weekly Update] 2020-02-01 ~ 2020-02-14

This is the Pulsar community weekly update for 2020-02-01 ~ 2020-02-14, with updates on refreshing authentication credentials, namespace level offloader, new bundle split algorithm to support evenly distributing topics, and many bug fixes and enhancements around helm chart.

### Development

- [PIP-55] Refresh authentication credentials.

    https://github.com/apache/pulsar/pull/6074

- [Client][Node] The first release candidate of Pulsar Node client version 1.1.0.

    https://lists.apache.org/thread.html/r12ae256d7b8ed91bb5436d9d35a5b70677a041c7558c77dd37740e65%40%3Cdev.pulsar.apache.org%3E
    
- [CI] A `pulsarbot` GitHub action is introduced for allowing contributors to re-run failed checks by commenting `/pulsarbot run-failure-checks`.

    https://lists.apache.org/thread.html/r425a963ce02d64d16d856938eed99f621958a5b238ea9fff9772d73c%40%3Cdev.pulsar.apache.org%3E
    
- [CI] CI related GitHub actions are now moved to [apache/pulsar-test-infra](https://github.com/apache/pulsar-test-infra).

    https://lists.apache.org/thread.html/r46bf4fdc524155863f314fd58f38567ae1ce9e6b14f1610368813fc0%40%3Cdev.pulsar.apache.org%3E

### Notable Feature

- [Broker] Namespace level offloader (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6183
    
- [Broker] Supports evenly distribute topics count when splits bundle (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6241

- [Broker] Add maxUnackedMessagesPerSubscription and maxUnackedMessagesPerConsumer on namespaces policies (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/5936

- [Broker] Support `unload` all partitions of a partitioned topic (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6187
    
- [Broker][Stats] Expose lastConsumedTimestamp and lastAckedTimestamp to consumer stats (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6051
    
- [Functions][Go] Add Go Function heartbeat (and gRPC service) for production usage (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6031

### Notable Bug Fix

- [ZooKeeper] Upgrade ZooKeeper to 3.5.7 to address split-brain issue (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6329

- [Broker][compaction] Fix log compaction for flow control/empty topic/last deletion (Release: 2.6.0, 2.5.1, 2.4.3).

    https://github.com/apache/pulsar/pull/6237
    
- [Broker] Fix bug that backlog message that has not yet expired could be deleted due to TTL (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6211

- [Helm] Several bug fixes and improvements have been made to current helm charts.

    https://github.com/apache/pulsar/pull/6158

    https://github.com/apache/pulsar/pull/6148

    https://github.com/apache/pulsar/pull/6160

    https://github.com/apache/pulsar/pull/6201

    https://github.com/apache/pulsar/pull/6280
    
    https://github.com/apache/pulsar/pull/6191
    
- [Client][Java] Fix get schema version in HttpLookupService. (Release: 2.6.0, 2.5.1)

    https://github.com/apache/pulsar/pull/6193
    
- [Client][Java] Flush the potential duplicated message when adding messages to a batch (Release: 2.6.0, 2.5.1)

    https://github.com/apache/pulsar/pull/6326

### Ecosystem

- [Client][DotNet] Pulsar.Client 0.13.0 released with multi hosts service URL support.

    https://www.nuget.org/packages/Pulsar.Client/

### Event / News

- [Survey] The Pulsar User Survey is closed on February 14. We have received 165 responses. The survey report will be published soon.

    https://forms.office.com/Pages/ResponsePage.aspx?id=DQSIkWdsW0yxEjajBLZtrQAAAAAAAAAAAAZAAOjIXw9UMUNLRUdJMVJBS1RRNjVNNjMzR0JPTFpGWi4u
    
- [Summit] The Call-for-Presentation for Pulsar Summit is closed on February 14. We have received 40 talk submissions. The conference schedule will be published soon.

    https://twitter.com/PulsarSummit/status/1229465785308893186