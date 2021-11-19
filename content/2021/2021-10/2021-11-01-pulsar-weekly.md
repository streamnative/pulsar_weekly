---
title: "2021-11-01-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-10-25 ~ 2021-10-31"
date: 2021-10-25 ~ 2021-10-31
description: "This is the Pulsar community weekly update for 2021-10-25 ~ 2021-10-31, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-11-01-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-10-25 ~ 2021-10-31

This is the Pulsar community weekly update for 2021-10-25 ~ 2021-10-31, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[lordcheng10](https://github.com/lordcheng10), [LeBW](https://github.com/LeBW), [Demogorgon314](https://github.com/Demogorgon314), [codelipenghui](https://github.com/codelipenghui), [gaoran10](https://github.com/gaoran10), [lhotari](https://github.com/lhotari), [timmyyuan](https://github.com/timmyyuan), [congbobo184](https://github.com/congbobo184), [merlimat](https://github.com/merlimat), [gaozhangmin](https://github.com/gaozhangmin), [yuruguo](https://github.com/yuruguo), [MarvinCai](https://github.com/MarvinCai), [zeo1995](https://github.com/zeo1995), [michaeljmarshall](https://github.com/michaeljmarshall), [urfreespace](https://github.com/urfreespace), [amarlearning](https://github.com/amarlearning), [ericsyh](https://github.com/ericsyh), [Shoothzj](https://github.com/Shoothzj), [fengtao1998](https://github.com/fengtao1998), [yangl](https://github.com/yangl)

## Pulsar Program Overview
- Github Forks: 2.5k
- Github Stars: 9.8k
- Github Contributors: 461

## Pulsar Updates

### Highlights
 
- [Pulsar Admin] Add support for resetting subscription to `Earliest` or `Latest`.
<br>https://github.com/apache/pulsar/pull/12302 
<br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Python Client] Support using a custom Avro schema definition on Python Client.
<br>https://github.com/apache/pulsar/pull/12516 
<br>by [gaoran10](https://github.com/gaoran10)

### Notable Features
- [Pulsar SQL] Set `NettyMaxFrameSizeBytes` on Pulsar SQL for the BookKeeper client to allow users Pulsar SQL query big entry data.
<br>https://github.com/apache/pulsar/pull/12448 
<br>by [gaoran10](https://github.com/gaoran10)
- [Client] Update producer stats when producer `cancelStatsTimeout`.<br>https://github.com/apache/pulsar/pull/12500
<br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Python Client]  Python Client support using a custom Avro schema definition.
<br>https://github.com/apache/pulsar/pull/12516 
<br>[gaoran10](https://github.com/gaoran10)
- [Pulsar Admin] Add support for resetting subscription to `Earliest` or `Latest`.
<br>https://github.com/apache/pulsar/pull/12302 
<br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Metadata] Allow different instances `LocalMemoryMetadataStore` that share the same state.
<br>https://github.com/apache/pulsar/pull/12390 
<br>by [merlimat](https://github.com/merlimat))
### Notable Bug Fix
- [Broker] Allow to delete the authentication policies when deleting topic.<br>https://github.com/apache/pulsar/pull/12215
<br>by [LeBW](https://github.co`m/LeBW)
- [Broker] Fix the batch message ACK for the WebSocket proxy.<br>https://github.com/apache/pulsar/pull/12530 
<br>by [codelipenghui](https://github.com/codelipenghui)
- [Broker] Fix the issue that Websocket didn't pass the encryption context to consumers.
<br>https://github.com/apache/pulsar/pull/12539 
<br>by [merlimat](https://github.com/merlimat)
- [Broker] Fix the issue that `MessageDeduplication` with Producer Name can not be cleaned up.
<br>https://github.com/apache/pulsar/pull/12493 
<br>by [congbobo184](https://github.com/congbobo184)
- [Java Client] Remove data race in `MultiTopicsConsumerImpl` to ensure correct message order.
<br>https://github.com/apache/pulsar/pull/12456 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Broker] Fix the retry topic's `REAL_TOPIC` & `ORIGIN_MESSAGE_ID` property.
<br>https://github.com/apache/pulsar/pull/12451 
<br>by [yangl](https://github.com/yangl)
- [Broker] Fix the race of `delete subscription` and `delete topic`.
<br>https://github.com/apache/pulsar/pull/12240 
<br>by [Shoothzj](https://github.com/Shoothzj)


## Events / News
- Past Events
   - [Utilizing Apache Pulsar, Apache NiFi and MiNiFi for EdgeAI IoT at Scale](https://www.slideshare.net/bunkertor/ai-dev-world-utilizing-apache-pulsar-apache-ni-fi-and-minifi-for-edgeai-iot-at-scale)
    - Flink Forward Global Virtual Conference 2021
        - [Interactive Session: AMA | Pulsar and Flink for Unified Data Processing](https://www.youtube.com/watch?v=sl1d7vZYe1E)
        - [Continuous Queries on Apache Pulsar using Flink SQL](https://www.youtube.com/watch?v=iWn_BI1c9m4&list=PLDX4T_cnKjD0J2LFr7yBk2aSS_o2l-7ue&index=50)
- Upcoming Events
    - [Pulsar Summit Asia 2021](https://hopin.com/events/pulsar-summit-asia-2021)
    - DevFest 2021 UK & Ireland
        - [Using Apache NiFi with Apache Pulsar for Fast Data On-Ramp](https://www.devfest-uki.com/) by Timothy Spann