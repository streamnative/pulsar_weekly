---
title: "2022-02-21-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-02-14 ~ 2022-02-20"
date: 2022-02-14 ~ 2022-02-20
description: "This is the Pulsar community weekly update for 2022-02-14 ~ 2022-02-20, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-02-21-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-02-14 ~ 2022-02-20

This is the Pulsar community weekly update for 2022-02-14 ~ 2022-02-20, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[Technoboy-](https://github.com/Technoboy-), [yaalsn](https://github.com/yaalsn), [lhotari](https://github.com/lhotari), [merlimat](https://github.com/merlimat), [dave2wave](https://github.com/dave2wave), [sijie](https://github.com/sijie), [gaozhangmin](https://github.com/gaozhangmin), [mattisonchao](https://github.com/mattisonchao), [michaeljmarshall](https://github.com/michaeljmarshall), [315157973](https://github.com/315157973), [wangjialing218](https://github.com/wangjialing218), [Anonymitaet](https://github.com/Anonymitaet), [momo-jun](https://github.com/momo-jun), [Shoothzj](https://github.com/Shoothzj), [EronWright](https://github.com/EronWright), [liangyepianzhou](https://github.com/liangyepianzhou), [nicoloboschi](https://github.com/nicoloboschi), [yuruguo](https://github.com/yuruguo), [Jason918](https://github.com/Jason918), [nodece](https://github.com/nodece), [Demogorgon314](https://github.com/Demogorgon314), [rdhabalia](https://github.com/rdhabalia), [lordcheng10](https://github.com/lordcheng10), [AnonHxy](https://github.com/AnonHxy), [aloyszhang](https://github.com/aloyszhang), [RocMarshal](https://github.com/RocMarshal), [zhaoyajun2009](https://github.com/zhaoyajun2009), [RobertIndie](https://github.com/RobertIndie), [HQebupt](https://github.com/HQebupt), [congbobo184](https://github.com/congbobo184)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Highlights
- [Client] Create init subscription before sending message to DLQ.
  <br>https://github.com/apache/pulsar/pull/13355 
  <br>by [RobertIndie](https://github.com/RobertIndie)
- [Broker] Redeliver command and add an epoc. 
  <br>https://github.com/apache/pulsar/pull/10478 
  <br>by [congbobo184](https://github.com/congbobo184)
- [Function] Add funtion API to support preloading and releasing external resources.
  <br>https://github.com/apache/pulsar/pull/13205 
  <br>by [wangjialing218](https://github.com/wangjialing218)

### Notable Features
- [Doc] Add doc for cluster-level failover.
  <br>https://github.com/apache/pulsar/pull/14314 
  <br>by [Anonymitaet](https://github.com/Anonymitaet)
- [Transaction] Add auth for `PerformanceTransaction`.
  <br>https://github.com/apache/pulsar/pull/14271 
  <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Broker] Optimize topic policy on `HierarchyTopicPolicies` with `publishRate`.
  <br>https://github.com/apache/pulsar/pull/14267 
  <br>by [AnonHxy](https://github.com/AnonHxy)
- [Pulsar Client] Log producer batchSize and msgSize percentiles.
  <br>https://github.com/apache/pulsar/pull/14229 
  <br>by [AnonHxy](https://github.com/AnonHxy)
- [CI] Update `.asf.yaml` to protect release branches.
  <br>https://github.com/apache/pulsar/pull/14226 
  <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Broker] Move `schema compatibility strategy` cmd from `topics` to `topicPolicies`.
  <br>https://github.com/apache/pulsar/pull/14225 
  <br>by [nodece](https://github.com/nodece)
- [Broker] Optimize topic policy with `HierarchyTopicPolicies`.
  <br>https://github.com/apache/pulsar/pull/14151 
  <br>by [AnonHxy](https://github.com/AnonHxy)
- [Docker Image] Update the Pulsar docker images to run as a non-root user by default.
  <br>https://github.com/apache/pulsar/pull/13376 
  <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Client] Create init subscription before sending message to DLQ. 
  <br>https://github.com/apache/pulsar/pull/13355 
  <br>by [RobertIndie](https://github.com/RobertIndie)
- [Configuraiton] Reconnect broker when ZooKeeper session expires.
  <br>https://github.com/apache/pulsar/pull/13341 
  <br>by [HQebupt](https://github.com/HQebupt)
- [Function] Add Funtion API to support preloading and releasing external resources.
  <br>https://github.com/apache/pulsar/pull/13205 
  <br>by [wangjialing218](https://github.com/wangjialing218)
- [Broker] Redeliver command and add an epoch.
  <br>https://github.com/apache/pulsar/pull/10478 
  <br>by [congbobo184](https://github.com/congbobo184)

### Notable Bug Fix
- [Broker] Optimize the process of finding the NICs.
  <br>https://github.com/apache/pulsar/pull/14340 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [CI] Protect branch-2.10 from force pushes.
  <br>https://github.com/apache/pulsar/pull/14334 
  <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Websocket] Fix `ClassCastException` when user creates `MultiTopicReader`.
  <br>https://github.com/apache/pulsar/pull/14316 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Fix the issue that `CommandLookupTopic.advertisedListenerName` may be blank.
  <br>https://github.com/apache/pulsar/pull/14306 
  <br>by [EronWright](https://github.com/EronWright)
- [Client] Fix a mismatch of time units in `errMsg` when producer fails to send.
  <br>https://github.com/apache/pulsar/pull/14299 
  <br>by [Jason918](https://github.com/Jason918)
- [Broker] Fix NPE in `internalSkipMessages`.
  <br>https://github.com/apache/pulsar/pull/14297 
  <br>by [nodece](https://github.com/nodece)
- [CI] Fix error in `IntelliJ` when running tests.
  <br>https://github.com/apache/pulsar/pull/14296 
  <br>by [lhotari](https://github.com/lhotari)
- [Broker] Fix `TopicPoliciesCacheNotInitException` .
  <br>https://github.com/apache/pulsar/pull/14293 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker]  Fix the issue that the batch ack count is negtive.
  <br>https://github.com/apache/pulsar/pull/14288 
  <br>by [Technoboy-](https://github.com/Technoboy-)
- [Metadata] Fix metadata cache inconsistency on refresh.
  <br>https://github.com/apache/pulsar/pull/14283 
  <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Broker] Fix ack-hole and backlog for `persistent-replicator`.
  <br>https://github.com/apache/pulsar/pull/14282 
  <br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker]Fix invalid period 0.0 to calculate rate.
  <br>https://github.com/apache/pulsar/pull/14280 
  <br>by [lordcheng10](https://github.com/lordcheng10)
- [Transaction] Change to `STATE_UPDATER.set(this, State.Close);`.
  <br>https://github.com/apache/pulsar/pull/14277 
  <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Broker] Fix `validateGlobalNamespaceOwnership` wrap exception.
  <br>https://github.com/apache/pulsar/pull/14269 
  <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Clean up individually deleted messages before the mark-delete position.
  <br>https://github.com/apache/pulsar/pull/14261 
  <br>by [merlimat](https://github.com/merlimat)
- [Broker] Fix `PersistentAcknowledgmentsGroupingTracker` set BitSet.
  <br>https://github.com/apache/pulsar/pull/14260 
  <br>by [Technoboy-](https://github.com/Technoboy-)
- [Management] Fix the issue that `RestAPI` might print an error log when the server returns the redirect code(307).
  <br>https://github.com/apache/pulsar/pull/14259 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Depandency] Upgrade Netty from 4.1.73.Final to 4.1.74.Final.
  <br>https://github.com/apache/pulsar/pull/14257 
  <br>by [Shoothzj](https://github.com/Shoothzj)
- [Broker] Fix the issue that rackaware placement policy does not take effect after deleting rack configuration.
  <br>https://github.com/apache/pulsar/pull/14248 
  <br>by [aloyszhang](https://github.com/aloyszhang)
- [Test Client] Add short name `cf` for long parameter name `conf-file`.
  <br>https://github.com/apache/pulsar/pull/14245 
  <br>by [RocMarshal](https://github.com/RocMarshal)
- [Admin] Add short name for full name in Admin CLI.
  <br>https://github.com/apache/pulsar/pull/14301 
  <br>by [yuruguo](https://github.com/yuruguo)
- [Broker] Fix NPE of `internalExpireMessagesByTimestamp`.
  <br>https://github.com/apache/pulsar/pull/14243 
  <br>by [nodece](https://github.com/nodece)
- [Broker] Remove duplicated filter for `UniformLoadShedder#findBundlesForUnloading`.
  <br>https://github.com/apache/pulsar/pull/14198 
  <br>by [aloyszhang](https://github.com/aloyszhang)
- [Broker] Fix the issue that there are many Error messages in the broker.
  <br>https://github.com/apache/pulsar/pull/14196 
  <br>by [Demogorgon314](https://github.com/Demogorgon314)


## Resources 
### Blog
- [The Critical Role Streaming Plays in a Data Stack](https://foojay.io/today/the-critical-role-streaming-plays-in-a-data-stack/)

### Video
- [Supporting the entire lifecycle of Streaming Data](https://www.youtube.com/watch?v=CAk33ATlBXU)
- [Using the FLiPN Stack for Edge AI (Flink, NiFi, Pulsar)](https://www.youtube.com/watch?v=zlSbJxrmgh0)
- [Deploying Machine Learning Models with Pulsar Functions](https://www.youtube.com/watch?v=eRDG-xkY_Aw)

## Release
- [Apache/Pulsar-Client-Go v0.8.0](https://github.com/apache/pulsar-client-go/releases/tag/v0.8.0)

## Events / News
- Survey
    - [[5-min Survey] New Apache Pulsar Website](https://forms.office.com/pages/responsepage.aspx?id=DQSIkWdsW0yxEjajBLZtrQAAAAAAAAAAAAZAAOjIXw9UMFkzWUM0Q0JVSEtXWVY3SlM0UUMzQkxJVC4u)

- Past events
    - Community Conference 2022
        - [Ingesting Data at Scale into Elasticsearch with Apache Pulsar](https://www.youtube.com/watch?v=h_WfuyoGpaM)

- Upcoming events
    - 8 April, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - 17 May, 2022: Kubernetes Batch + HPC Day Europe
        - [Fast Data on-Ramp with Apache Pulsar on K8](https://kubernetesbatchdayeu22.sched.com/event/10F0q)
    - 18-20 July, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
