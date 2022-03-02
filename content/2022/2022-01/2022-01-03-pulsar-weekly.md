---
title: "2022-01-03-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-12-27 ~ 2022-01-02"
date: 2021-12-27 ~ 2022-01-02
description: "This is the Pulsar community weekly update for 2021-12-27 ~ 2022-01-02, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-01-03-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-12-27 ~ 2022-01-02

This is the Pulsar community weekly update for 2021-12-27 ~ 2022-01-02, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[aloyszhang](https://github.com/aloyszhang), [ericsyh](https://github.com/ericsyh), [lhotari](https://github.com/lhotari), [RobertIndie](https://github.com/RobertIndie), [Anonymitaet](https://github.com/Anonymitaet), [urfreespace](https://github.com/urfreespace), [mattisonchao](https://github.com/mattisonchao), [315157973](https://github.com/315157973), [fu-turer](https://github.com/fu-turer), [Shoothzj](https://github.com/Shoothzj), [Jason918](https://github.com/Jason918), [liudezhi2098](https://github.com/liudezhi2098), [codelipenghui](https://github.com/codelipenghui), [tjiuming](https://github.com/tjiuming), [BewareMyPower](https://github.com/BewareMyPower), [leizhiyuan](https://github.com/leizhiyuan), [gaoran10](https://github.com/gaoran10), [nodece](https://github.com/nodece)

## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.4k
- Github Contributors: 509

## Pulsar Updates
### Highlights
- [Security] Upgrade Log4j to 2.17.1.
 <br>https://github.com/apache/pulsar/pull/13552 
 <br>by [lhotari](https://github.com/lhotari)
- [Client] Introduce chunk message ID. 
 <br>https://github.com/apache/pulsar/pull/12403 
 <br>by [RobertIndie](https://github.com/RobertIndie)
 
### Notable Features
- [Broker] Subscribe rate support cross multiple clusters.
 <br>https://github.com/apache/pulsar/pull/13561 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker] Message dispatch rate policies support cross multiple clusters.
 <br>https://github.com/apache/pulsar/pull/13511 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Delayed delivery policy support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13550 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Max unacked messages on subscription support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13549 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Compaction threshold policies support cross multiple clusters. 
 <br>https://github.com/apache/pulsar/pull/13513 
 <br>by [mattisonchao](https://github.com/mattisonchao)
 
### Notable Bug Fix
- [Broker] Fix the issue that producer create failed with `connectionFailed` will leak some resource. 
 <br>https://github.com/apache/pulsar/pull/13505 
 <br>by [aloyszhang](https://github.com/aloyszhang)
- [Broker] In `MultiRolesTokenAuthorizationProvider.authorize`, return false immediately when the roles are empty.
 <br>https://github.com/apache/pulsar/pull/13477 
 <br>by [RobertIndie](https://github.com/RobertIndie)
- [BookKeeper] Fix the issue that `StatsBuckets addAll` use count as sum. 
 <br>https://github.com/apache/pulsar/pull/13467 
 <br>by [leizhiyuan](https://github.com/leizhiyuan)
- [Broker] Subscribe rate support cross multiple clusters.
 <br>https://github.com/apache/pulsar/pull/13561 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker] Fix getting the last message-id from an empty compact ledger. 
 <br>https://github.com/apache/pulsar/pull/13476 
 <br>by [gaoran10](https://github.com/gaoran10)
- [Broker] Return message ID from compacted ledger while the compaction cursor reaches the end of the topic. 
 <br>https://github.com/apache/pulsar/pull/13533 
 <br>by [codelipenghui](https://github.com/codelipenghui)
 
 ### Ecosystem
- [Pulsar SQL] Support for protobuf/timestamp. 
 <br>https://github.com/apache/pulsar/pull/13287 
 <br>by [tjiuming](https://github.com/tjiuming)

 
## Blog
- [Building Applications with Apache Spark and Apache Pulsar](https://medium.com/@tspann/building-applications-with-apache-spark-and-apache-pulsar-87a9611f0fd9)

## Events / News
- Upcoming events
    - March 10, 2022: FliPN Stack for Cloud Data Lakes | Meetup
        - [Using Apache Pulsar, Flink, and Nifi to Stream to Your Data Lakes](https://streamnative.io/en/event/meetup-flipn-stack-for-cloud-data-lakes/)
    - March 11, 2022: Virtual Meetup
        - [FLiPN Stack for Cloud Data Lakes: Using Apache Pulsar™, Apache Flink®, and Apache Nifi® to Stream to your Data Lake](https://www.meetup.com/new-york-city-apache-pulsar-meetup/events/283837865/)
    - March 23,2022: Live Webinar
        - [Event Streaming with Apache Pulsar and Kotlin](https://info.jetbrains.com/kotlin-webinar-march22-2022.html?)
