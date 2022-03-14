---
title: "2021-12-27-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-12-20 ~ 2021-12-26"
date: 2021-12-20 ~ 2021-12-26
description: "This is the Pulsar community weekly update for 2021-12-20 ~ 2021-12-26, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-12-27-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-12-20 ~ 2021-12-26

This is the Pulsar community weekly update for 2021-12-20 ~ 2021-12-26, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[Shawyeok](https://github.com/Shawyeok), [Demogorgon314](https://github.com/Demogorgon314), [nicoloboschi](https://github.com/nicoloboschi), [liangyepianzhou](https://github.com/liangyepianzhou), [rdhabalia](https://github.com/rdhabalia), [BewareMyPower](https://github.com/BewareMyPower), [nodece](https://github.com/nodece), [zymap](https://github.com/zymap), [315157973](https://github.com/315157973), [ericsyh](https://github.com/ericsyh), [Anonymitaet](https://github.com/Anonymitaet), [Shoothzj](https://github.com/Shoothzj), [michaeljmarshall](https://github.com/michaeljmarshall), [lhotari](https://github.com/lhotari), [eolivelli](https://github.com/eolivelli), [urfreespace](https://github.com/urfreespace), [kijanowski](https://github.com/kijanowski), [yannick](https://github.com/yannick), [tomscut](https://github.com/tomscut), [yuruguo](https://github.com/yuruguo)

## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.4k
- Github Contributors: 509

## Pulsar Updates
### Highlights
- [Transaction] Add the `CmdTransactions` to `PulsarAdminTool`.
 <br>https://github.com/apache/pulsar/pull/13447 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
 
### Notable Features
- [Broker] Load-balancer support disabling max-session for bundle split. 
 <br>https://github.com/apache/pulsar/pull/13108 
 <br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker] Subscription types support across multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13482 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Deduplication status support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13487 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Message TTL support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13484 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Persistence topic policies support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13483 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Backlog quota support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13445 
 <br>by [315157973](https://github.com/315157973)
 
### Notable Bug Fix
- [Broker] Fix dead loop in `BacklogQuotaManager.dropBacklogForTimeLimit`. 
 <br>https://github.com/apache/pulsar/pull/13249 
 <br>by [Shawyeok](https://github.com/Shawyeok)
- [Client] Fix multi topic reader `hasmessageavailable` behavior. 
 <br>https://github.com/apache/pulsar/pull/13332 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Broker] Fix race conditions in closing producers and consumers. 
 <br>https://github.com/apache/pulsar/pull/13428 
 <br>by [lhotari](https://github.com/lhotari)

 
## Blog
- [Information Regarding Log4j Security Vulnerabilities](https://streamnative.io/blog/engineering/log4-mitigation-en/)

## Release 
- [Apache Pulsar 2.9.1](https://pulsar.apache.org/release-notes/)
- [Apache Pulsar NodeJS Client 1.5.0](https://github.com/apache/pulsar-client-node/releases)

## Events
- Upcoming events
    - March 10, 2022: FliPN Stack for Cloud Data Lakes | Meetup
        - [Using Apache Pulsar, Flink, and Nifi to Stream to Your Data Lakes](https://streamnative.io/en/event/meetup-flipn-stack-for-cloud-data-lakes/)
    - March 11, 2022: Virtual Meetup
        - [FLiPN Stack for Cloud Data Lakes: Using Apache Pulsar™, Apache Flink®, and Apache Nifi® to Stream to your Data Lake](https://www.meetup.com/new-york-city-apache-pulsar-meetup/events/283837865/)
    - March 23,2022: Live Webinar
        - [Event Streaming with Apache Pulsar and Kotlin](https://info.jetbrains.com/kotlin-webinar-march22-2022.html?)
