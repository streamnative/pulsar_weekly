---
title: "2022-02-07-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-01-31 ~ 2022-02-06"
date: 2022-01-31 ~ 2022-02-06
description: "This is the Pulsar community weekly update for 2022-01-31 ~ 2022-02-06, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-02-07-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-01-31 ~ 2022-02-06

This is the Pulsar community weekly update for 2022-01-31 ~ 2022-02-06, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[klevy-toast](https://github.com/klevy-toast), [eolivelli](https://github.com/eolivelli), [dave2wave](https://github.com/dave2wave), [nicoloboschi](https://github.com/nicoloboschi), [rdhabalia](https://github.com/rdhabalia), [mattisonchao](https://github.com/mattisonchao), [Jason918](https://github.com/Jason918), [merlimat](https://github.com/merlimat), [lhotari](https://github.com/lhotari), [Demogorgon314](https://github.com/Demogorgon314), [dlg99](https://github.com/dlg99), [BewareMyPower](https://github.com/BewareMyPower), [momo-jun](https://github.com/momo-jun)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Notable Features
- [Pulsar Client] Implement `--retain-key-ordering` for Sinks and Functions. 
 <br>https://github.com/apache/pulsar/pull/14083 
 <br>by [eolivelli](https://github.com/eolivelli)
- [Broker] Change sync method to async.
 <br>https://github.com/apache/pulsar/pull/14091 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Use custom media type `application/vnd.partitioned-topic-metadata+json` to distinguish the new content payload type.
 <br>https://github.com/apache/pulsar/pull/14117 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Add units test for `TableView`. 
 <br>https://github.com/apache/pulsar/pull/14100 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Funtions] Support specifying Ubuntu mirror for docker image builds. 
 <br>https://github.com/apache/pulsar/pull/14095 
 <br>by [lhotari](https://github.com/lhotari)
- [Pulsar IO] Add OWASP Dependency Checker to the GH CI workflows 
 <br>https://github.com/apache/pulsar/pull/13972 
 <br>by [dlg99](https://github.com/dlg99)
 
### Notable Bug Fix
- [Pulsar Client] Replace the use of `scheduleAtFixedRate` with `scheduleWithFixedDelay`. <br>https://github.com/apache/pulsar/pull/14125 
 <br>by [klevy-toast](https://github.com/klevy-toast)
- [Broker] Prevent `StackOverFlowException` in `KEY_SHARED` subscriptions. 
 <br>https://github.com/apache/pulsar/pull/14121 
 <br>by [eolivelli](https://github.com/eolivelli)
- [Proxy] Fix auto-cert refresh when proxy connects to broker.
 <br>https://github.com/apache/pulsar/pull/14130 
 <br>by [rdhabalia](https://github.com/rdhabalia)
- [Metadata] Skip the exception when the path `shortIdGenPath` has already been created by others.
 <br>https://github.com/apache/pulsar/pull/14118 
 <br>by [Jason918](https://github.com/Jason918)
- [Metadata] Fix the flaky-test `ZKSessionTest.testDisconnection`. 
 <br>https://github.com/apache/pulsar/pull/14129 
 <br>by [merlimat](https://github.com/merlimat)
- [Test] Replace the usage with `Awaitility`,
 <br>https://github.com/apache/pulsar/pull/14124 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Test] Fix the flaky-test `PerformanceProducerTest.testMsgKey`.
 <br>https://github.com/apache/pulsar/pull/14068 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Metadata] Fix the flaky-test `LockManagerTest.revalidateLockOnDifferentSession`. 
 <br>https://github.com/apache/pulsar/pull/14115 
 <br>by [merlimat](https://github.com/merlimat)
- [Test] Improve issue templates for flaky tests. 
 <br>https://github.com/apache/pulsar/pull/14116 
 <br>by [lhotari](https://github.com/lhotari)
- [Test] Change the test runtime options to get Mockito working with a minimal configuration.
 <br>https://github.com/apache/pulsar/pull/14099 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Functions] Fix the issue that distributed log metadata is not correctly initialized. 
 <br>https://github.com/apache/pulsar/pull/13891 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Test] Remove development packages from Pulsar's docker images 
 <br>https://github.com/apache/pulsar/pull/14093 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Add null check to avoid NPE.
 <br>https://github.com/apache/pulsar/pull/14090 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [JAVA Client] Fix the issue that `ConsumerBuilder: java.lang.IllegalArgumentException: properties` cannot be empty,
 <br>https://github.com/apache/pulsar/pull/14074 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [C++ Client] Fix the consumer configuration inconsistency with Java client.
 <br>https://github.com/apache/pulsar/pull/14070 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [C++ Client] Fix the consumer configuration inconsistency with Java client.
 <br>https://github.com/apache/pulsar/pull/14070 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)


## Resources 
### Blog
- [Integrating Apache Pulsar with BigQuery](https://streamnative.io/blog/engineering/2022-02-03-integrating-apache-pulsar-with-bigquery/)
- [Using Apache Pulsar WebSockets for Real-Time Messaging in Front-End Applications](https://medium.com/@tspann/using-apache-pulsar-websockets-for-real-time-messaging-in-front-end-applications-cf0ac2d80d10)
### Video
- [Real-Time Analytics with Apache Pulsar and Spark Streaming](https://www.youtube.com/watch?v=Ixh8PhGor1c)
- [Integrating Apache Pulsar with BiqQuery](https://www.youtube.com/watch?v=0Tx9B_iHKrI)
le.com/forms/d/e/1FAIpQLSfZLn3U2QqzXNEV0p4BoB6lSI88fOOuQYB_w59tEoe_uP684w/viewform)

## Events / News
- Survey
    - [[5-min Survey] New Apache Pulsar Website](https://forms.office.com/pages/responsepage.aspx?id=DQSIkWdsW0yxEjajBLZtrQAAAAAAAAAAAAZAAOjIXw9UMFkzWUM0Q0JVSEtXWVY3SlM0UUMzQkxJVC4u)

- Upcoming events
    - 8 April, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - 17 May, 2022: Kubernetes Batch + HPC Day Europe
        - [Fast Data on-Ramp with Apache Pulsar on K8](https://kubernetesbatchdayeu22.sched.com/event/10F0q)
    - 18-20 July, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
