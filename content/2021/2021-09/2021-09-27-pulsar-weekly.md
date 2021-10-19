---
title: "2021-09-27-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-09-20 ~ 2021-09-26"
date: 2021-09-20 ~ 2021-09-26
description: "This is the Pulsar community weekly update for 2021-09-20 ~ 2021-09-26, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-09-27-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-09-20 ~ 2021-09-26

This is the Pulsar community weekly update for 2021-09-20 ~ 2021-09-26, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[yuruguo](https://github.com/yuruguo), [lhotari](https://github.com/lhotari), [315157973](https://github.com/315157973), [massakam](https://github.com/massakam), [freeznet](https://github.com/freeznet), [nicoloboschi](https://github.com/nicoloboschi), [metahys](https://github.com/metahys), [hangc0276](https://github.com/hangc0276), [rdhabalia](https://github.com/rdhabalia), [merlimat](https://github.com/merlimat), [rdhabalia](https://github.com/rdhabalia), [fengtao1998](https://github.com/fengtao1998), [ericsyh](https://github.com/ericsyh), [addisonj](https://github.com/addisonj), [michaeljmarshall](https://github.com/michaeljmarshall), [Shoothzj](https://github.com/Shoothzj), [urfreespace](https://github.com/urfreespace)

## Pulsar Program Overview

- Github Forks: 2.4k
- Github Stars: 9.6k
- Github Contributors: 450

## Pulsar Updates

### Highlights

- [Broker] PIP-45: Removed access to ZooKeeper Client from `PulsarService`. 
<br>https://github.com/apache/pulsar/pull/12100 
<br>by [merlimat](https://github.com/merlimat)

- [Broker] PIP-45: Remove `ConfigurationCacheService`. 
<br>https://github.com/apache/pulsar/pull/12078 
<br>by [merlimat](https://github.com/merlimat)

- [Broker] Remove unnecessary authenticate method definition. 
<br>https://github.com/apache/pulsar/pull/12068 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

### Notable Features

- [Function] Support setting subscription position. 
<br>https://github.com/apache/pulsar/pull/11990 
<br>by [freeznet](https://github.com/freeznet)

- [C++] Support setting `ConsumerEventListener` in Pulsar CPP Client. 
<br>https://github.com/apache/pulsar/pull/12118 
<br>by [metahys](https://github.com/metahys)

- [IO] Remove the deprecated API usage in HDFS. 
<br>https://github.com/apache/pulsar/pull/12080 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [C++] Support setting priority for consumer. 
<br>https://github.com/apache/pulsar/pull/12076 
<br>by [metahys](https://github.com/metahys)

### Notable Bug Fix

- [Client] Fix `ConcurrentModificationException` in `sendAsync`. 
<br>https://github.com/apache/pulsar/pull/11884 
<br>by [lhotari](https://github.com/lhotari)

- [Broker] Fix the issue that when a compaction topic deletes a message, messages in `TopicPolicies` will never be cleaned up. 
<br>https://github.com/apache/pulsar/pull/11928 
<br>by [315157973](https://github.com/315157973)

- [Client] Fix the issue that `pulsar-client` command cannot consume v2 topics through WebSocket. 
<br>https://github.com/apache/pulsar/pull/12000 
<br>by [massakam](https://github.com/massakam)

- [BookKeeper] When disconnected, ManagedLedger will no longer attempt deferrable metadata operations.  
<br>https://github.com/apache/pulsar/pull/12101 
<br>by [merlimat](https://github.com/merlimat)

- [ZooKeeper] Fix the issue that `setConf` is called before `setBookieAddressResolver`. 
<br>https://github.com/apache/pulsar/pull/12097 
<br>by [addisonj](https://github.com/addisonj)

- [Client] Fix NPE when pulsar-storm bolt or any other client app tries to create message without initializing producer in it. 
<br>https://github.com/apache/pulsar/pull/12106 
<br>by [rdhabalia](https://github.com/rdhabalia)

- [Broker] Trigger unloading bundle when the ownership cache lock expires.  
<br>https://github.com/apache/pulsar/pull/12194 
<br>by [merlimat](https://github.com/merlimat)

## Blog
- [What’s New in Apache Pulsar 2.8.1](https://streamnative.io/blog/release/2021-09-23-pulsar-281/)
- 
## Events / News
- Upcoming Events
    - September 30th: [Apache Pulsar Meetup Japan](https://japan-pulsar-user-group.connpass.com/event/222026/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)

- Call For Participation
    - [Pulsar Summit Asia 2021 CFP is Open until 09/30](https://pulsar.apache.org/blog/2021/08/18/asia-cfp/)