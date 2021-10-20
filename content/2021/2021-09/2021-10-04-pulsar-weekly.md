---
title: "2021-10-04-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-09-27 ~ 2021-10-03"
date: 2021-09-27 ~ 2021-10-03
description: "This is the Pulsar community weekly update for 2021-09-27 ~ 2021-10-03, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-10-04-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-09-27 ~ 2021-10-03

This is the Pulsar community weekly update for 2021-09-27 ~ 2021-10-03, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[MarvinCai](https://github.com/MarvinCai), [yuruguo](https://github.com/yuruguo), [michaeljmarshall](https://github.com/michaeljmarshall), [urfreespace](https://github.com/urfreespace), [codelipenghui](https://github.com/codelipenghui), [freeznet](https://github.com/freeznet), [merlimat](https://github.com/merlimat), [michaeljmarshall](https://github.com/michaeljmarshall), [gaozhangmin](https://github.com/gaozhangmin), [BewareMyPower](https://github.com/BewareMyPower), [massakam](https://github.com/massakam), [baomingyu](https://github.com/baomingyu), [rdhabalia](https://github.com/rdhabalia), [dlg99](https://github.com/dlg99), [lordcheng10](https://github.com/lordcheng10), [315157973](https://github.com/315157973), [lhotari](https://github.com/lhotari), [eolivelli](https://github.com/eolivelli)

## Pulsar Program Overview
- Github Forks: 2.4k
- Github Stars: 9.6k
- Github Contributors: 451

## Pulsar Updates

### Highlights
- [Schema] PIP-45: Add the support for passing the path and stats of metadata value to serializer. 
<br>https://github.com/apache/pulsar/pull/12243 
<br>by [merlimat](https://github.com/merlimat)
- [Metadata] PIP-45: Revalidate the lock on `LockResource.updateValue()` if needed. 
<br>https://github.com/apache/pulsar/pull/12190 
<br>by [merlimat](https://github.com/merlimat)
- [Proxy] Add Proxy Extensions to Pulsar Proxy.
<br>https://github.com/apache/pulsar/pull/11838 
<br>by [eolivelli](https://github.com/eolivelli)

### Notable Features
- [Test] Add `totalmessages` when periodic prints throughput. 
<br>https://github.com/apache/pulsar/pull/12084 
<br>by [yuruguo](https://github.com/yuruguo)
- [Broker] Loadbalancer avoid offloading the heartbeat namespace. 
<br>https://github.com/apache/pulsar/pull/12252 
<br>by [codelipenghui](https://github.com/codelipenghui)
- [Python] Stop sorting schema fields by default. 
<br>https://github.com/apache/pulsar/pull/12232 
<br>by [merlimat](https://github.com/merlimat)
- [Java Client] Remove unnecessary stats incremement. 
<br>https://github.com/apache/pulsar/pull/12229 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Metrics] Add support for splitting topic and partition label in Prometheus. 
<br>https://github.com/apache/pulsar/pull/12225
<br>by [codelipenghui](https://github.com/codelipenghui)
- [Java Client] Remove unnecessary synchronizationand simplify initialization. 
<br>https://github.com/apache/pulsar/pull/12228 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Broker] Disable stats recorder for built-in Pulsar Client. 
<br>https://github.com/apache/pulsar/pull/12217 
<br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Broker] Remove redundant parameters of `additionalNumberOfMessages` in method `internalConsumerFlow`.
<br>https://github.com/apache/pulsar/pull/12188 
<br>by [lordcheng10](https://github.com/lordcheng10)
- [BookKeeper] Optimize the memory usage of Cache Eviction. 
<br>https://github.com/apache/pulsar/pull/12045 
<br>by [315157973](https://github.com/315157973)
- [Broker] PIP-64: Add produce message REST API. 
<br>https://github.com/apache/pulsar/pull/8125 
<br>by [MarvinCai](https://github.com/MarvinCai)
- [Admin] Add options to get precise backlog on v1 topic. 
<br>https://github.com/apache/pulsar/pull/8927 
<br>by [rdhabalia](https://github.com/rdhabalia)

## Events / News
- Past Events
    - October 6th: [Pulsar Virtual Summit Europe](https://pulsar-summit.org/en/event/europe-2021/schedule/first-day)
- Upcoming Events
    - November 20-21th: [Pulsar Summit Asia 2021](https://hopin.com/events/pulsar-summit-asia-2021)