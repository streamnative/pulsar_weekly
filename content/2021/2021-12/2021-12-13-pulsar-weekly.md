---
title: "2021-12-13-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-12-06 ~ 2021-12-12"
date: 2021-12-06 ~ 2021-12-12
description: "This is the Pulsar community weekly update for 2021-12-06 ~ 2021-12-12, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-12-13-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-12-06 ~ 2021-12-12

This is the Pulsar community weekly update for 2021-12-06 ~ 2021-12-12, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[wuzhanpeng](https://github.com/wuzhanpeng), [Demogorgon314](https://github.com/Demogorgon314), [michaeljmarshall](https://github.com/michaeljmarshall), [Technoboy-](https://github.com/Technoboy-), [hangc0276](https://github.com/hangc0276), [MMirelli](https://github.com/MMirelli), [billowqiu](https://github.com/billowqiu), [liangyepianzhou](https://github.com/liangyepianzhou), [tsturzl](https://github.com/tsturzl), [lhotari](https://github.com/lhotari), [congbobo184](https://github.com/congbobo184), [BewareMyPower](https://github.com/BewareMyPower), [nicoloboschi](https://github.com/nicoloboschi), [codelipenghui](https://github.com/codelipenghui), [cbornet](https://github.com/cbornet), [LeBW](https://github.com/LeBW), [Jason918](https://github.com/Jason918), [merlimat](https://github.com/merlimat), [yuruguo](https://github.com/yuruguo), [eolivelli](https://github.com/eolivelli), [zwalsh-toast](https://github.com/zwalsh-toast), [mattisonchao](https://github.com/mattisonchao)

## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.4k
- Github Contributors: 505

## Pulsar Updates
### Highlights
- Apache Pulsar 2.9.0 is released.
 <br>https://github.com/apache/pulsar/pull/12425 
 <br>by [eolivelli](https://github.com/eolivelli)
- [Blog] Add blog post to explain workaround for log4j security issue.
 <br>https://github.com/apache/pulsar/pull/13242 
 <br>by [merlimat](https://github.com/merlimat)
- [C++ Client] Add blog post to explain workaround for Log4j security issue.
 <br>https://github.com/apache/pulsar/pull/13246 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Security] Upgrade OkHttp3 to address CVE-2021-0341.
 <br>https://github.com/apache/pulsar/pull/13065 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
 
 
### Notable Features
- [Java Client] Allow consumer to be created in a paused state.
 <br>https://github.com/apache/pulsar/pull/11974 
 <br>by [zwalsh-toast](https://github.com/zwalsh-toast)
- [Broker] Use current `resourceUsage` value as `historyUsage` when leader changes in `ThresholdShedder`. 
 <br>https://github.com/apache/pulsar/pull/13136 
 <br>by [hangc0276](https://github.com/hangc0276)
- [BookKeeper] Update cursor last active timestamp .
 <br>https://github.com/apache/pulsar/pull/13166 
 <br>by [wuzhanpeng](https://github.com/wuzhanpeng)
- [Broker] Add`managedLedgerOffloadBucket` to `broker.conf`.
 <br>https://github.com/apache/pulsar/pull/12173 
 <br>by [MMirelli](https://github.com/MMirelli)
- [Java Client] Use Epoch to version producer's CNX to prevent early delivery of messages. 
 <br>https://github.com/apache/pulsar/pull/12779 
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [BookKeeper] Add a metric to show the timestamp from `the publish time of the earliest message in the backlog` to `the current time`.
 <br>https://github.com/apache/pulsar/pull/12523 
 <br>by [LeBW](https://github.com/LeBW)
- [Broker] Add `removeMaxConsumersPerSubscription` method for `v1 namespace`. 
 <br>https://github.com/apache/pulsar/pull/13192 
 <br>by [yuruguo](https://github.com/yuruguo)
- [Broker] Use current `resourceUsage` value as `historyUsage` when leader change in `ThresholdShedder`. 
 <br>https://github.com/apache/pulsar/pull/13136 
 <br>by [hangc0276](https://github.com/hangc0276)
 
### Notable Bug Fix
- [Pulsar Client] Add Wireshark CMakefile and fix `pulsarDissector.cc` to make it build success.
 <br>https://github.com/apache/pulsar/pull/13236 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Broker] Fix flaky test for `BrokerServiceLookupTest.testModularLoadManagerSplitBundle`. https://github.com/apache/pulsar/pull/13159 
 <br>by [wuzhanpeng](https://github.com/wuzhanpeng)
- [Broker] Fix the issuee that when deleting topic with `NotFoundException`, it does not return to client. 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Pulsar Client] Fix th issue that fail to install in Mac client.
 https://github.com/apache/pulsar/pull/13193 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Pulsar Client] Fix the issue that CPP SDK did not respond to request 307 during lookup.
 <br>https://github.com/apache/pulsar/pull/13112 
 <br>by [billowqiu](https://github.com/billowqiu) 
- [Proxy] Fix the issue that the Pulsar proxy fails to start when deploying the master branch version with the Apache Pulsar Helm chart.
 <br>https://github.com/apache/pulsar/pull/13171 
 <br>by [lhotari](https://github.com/lhotari)
- [Transaction] Fix transaction sequenceId generate error. 
 <br>https://github.com/apache/pulsar/pull/13209 
 <br>by [congbobo184](https://github.com/congbobo184)
- [Client] Call `recycle()` to recycle the `MessagePayloadContextImpl` object in `recycle()` method.
 <br>https://github.com/apache/pulsar/pull/13233 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Transaction] Fix generate transactionId some comments. 
 <br>https://github.com/apache/pulsar/pull/13234 
 <br>by [congbobo184](https://github.com/congbobo184)
- [Broker] Fix a namespace policy override that was ignored when creating subscriptions. 
 <br>https://github.com/apache/pulsar/pull/12699 
 <br>by [cbornet](https://github.com/cbornet)
- [Java Client] Fix the issue that `parseProtobufSchema` method would be called twice. 
 <br>https://github.com/apache/pulsar/pull/13163 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Optimize `ManagedLedger`.
 <br>https://github.com/apache/pulsar/pull/13222
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- Fix the build issue if there is no maven cache.
 <br>https://github.com/apache/pulsar/pull/13248 
 <br>by [codelipenghui](https://github.com/codelipenghui)
- Add basic DOAP file for Pulsar. 
 <br>https://github.com/apache/pulsar/pull/11864 
 <br>by [eolivelli](https://github.com/eolivelli)
- [Transaction] Add a check for uninitialized PendingAck. 
 <br>https://github.com/apache/pulsar/pull/13088 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Python Client] Fix the issue that `JsonSchema` encoding is not idempotent. 
 <br>https://github.com/apache/pulsar/pull/12490 
 <br>by [tsturzl](https://github.com/tsturzl)
- [Broker] Add new field `messageTTLInSeconds` to `org.apache.pulsar.broker.service.AbstractTopic#topicPolicies`.
 <br>https://github.com/apache/pulsar/pull/13241 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker] Replace `BaseResources#deleteRecursiveAsync` with `MetadataStore#deleteRecursive`. 
 <br>https://github.com/apache/pulsar/pull/13240 
 <br>by [Jason918](https://github.com/Jason918)
- [Java Client] Send the `CloseProducer` before sending a command to recreate the `Producer`.
 <br>https://github.com/apache/pulsar/pull/13161 
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)

## Blog
- [Pulsar Hits 10,000 GitHub Stars Milestone](https://streamnative.io/blog/community/2021-12-07-pulsar-hits-10000-github-stars-milestone/)

## Events
- Past events
    - Embedded Fest 2021
        - [Using Apache Pulsar to provide real-time analytics on the edge](https://www.youtube.com/watch?v=o22U4DR8_ik)
- Upcoming events
    - March 10, 2022: FliPN Stack for Cloud Data Lakes | Meetup
        - [Using Apache Pulsar, Flink, and Nifi to Stream to Your Data Lakes](https://streamnative.io/en/event/meetup-flipn-stack-for-cloud-data-lakes/)
    - March 11, 2022: Virtual Meetup
        - [FLiPN Stack for Cloud Data Lakes: Using Apache Pulsar™, Apache Flink®, and Apache Nifi® to Stream to your Data Lake](https://www.meetup.com/new-york-city-apache-pulsar-meetup/events/283837865/)
    - March 23,2022: Live Webinar
        - [Event Streaming with Apache Pulsar and Kotlin](https://info.jetbrains.com/kotlin-webinar-march22-2022.html?)