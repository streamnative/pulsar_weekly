---
title: "2022-03-14-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-03-07 ~ 2022-03-13"
date: 2022-03-07 ~ 2022-03-13
description: "This is the Pulsar community weekly update for 2022-03-07 ~ 2022-03-13, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-03-14-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-03-07 ~ 2022-03-13

This is the Pulsar community weekly update for 2022-03-07 ~ 2022-03-13, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[Technoboy-](https://github.com/Technoboy-), [BewareMyPower](https://github.com/BewareMyPower), [wuxuanqicn](https://github.com/wuxuanqicn), [michaeljmarshall](https://github.com/michaeljmarshall), [zhaoyajun2009](https://github.com/zhaoyajun2009), [momo-jun](https://github.com/momo-jun), [gaozhangmin](https://github.com/gaozhangmin), [tuhaihe](https://github.com/tuhaihe), [shibd](https://github.com/shibd), [nodece](https://github.com/nodece), [mattisonchao](https://github.com/mattisonchao), [merlimat](https://github.com/merlimat), [nicoloboschi](https://github.com/nicoloboschi), [aloyszhang](https://github.com/aloyszhang), [Anonymitaet](https://github.com/Anonymitaet), [lhotari](https://github.com/lhotari), [urfreespace](https://github.com/urfreespace)
## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.5k
- Github Contributors: 514

## Pulsar Updates
### Highlights
- [Broker] Support split bundle by specified boundaries.
 <br>https://github.com/apache/pulsar/pull/13796 
 <br>by [aloyszhang](https://github.com/aloyszhang)

### Notable Features
- [Broker] Add log to track negtive unacked message.
 <br>https://github.com/apache/pulsar/pull/14501 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Support split bundle by specified boundaries.
 <br>https://github.com/apache/pulsar/pull/13796 
 <br>by [aloyszhang](https://github.com/aloyszhang)


### Notable Bug Fix
- [Broker] Fix lost message issue due to ledger rollover.
 <br>https://github.com/apache/pulsar/pull/14664 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [C++ Client] Fix thread safety issues for multi topic consumers.
 <br>https://github.com/apache/pulsar/pull/14380 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Tests] Fix the flaky test `MemoryLimitTest#testRejectMessages`.
 <br>https://github.com/apache/pulsar/pull/14628 
 <br>by [wuxuanqicn](https://github.com/wuxuanqicn)
- [Broke] Return `403` to the user when permission is denied.
 <br>https://github.com/apache/pulsar/pull/14638 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Fix inconsistent prompt messages when schema version is empty.
 <br>https://github.com/apache/pulsar/pull/14626 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Fix NPE when `packagemanagement` service is enabled in `standaloneService`.
 <br>https://github.com/apache/pulsar/pull/14500 
 <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Broker] Delete dead broker's broker-time-average metadata.
 <br>https://github.com/apache/pulsar/pull/14411 
 <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Broker] Fix the flaky test `NamespacesTest.testDeleteNamespaceWithBundles`.
 <br>https://github.com/apache/pulsar/pull/14552 
 <br>by [shibd](https://github.com/shibd)
- [C++ Client] Fix wrong units of Access Token Response's `expires_in` field.
 <br>https://github.com/apache/pulsar/pull/14554 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Broker] Fix wrong behaviour caused by failure to clean up the topic policy service state.
 <br>https://github.com/apache/pulsar/pull/14503 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [C++ Client] Handle exceptions for creating sockets when the file descriptor limit is reached.
 <br>https://github.com/apache/pulsar/pull/14587 
 <br>by [merlimat](https://github.com/merlimat)
- [Broker] Fix system topic replicate.
 <br>https://github.com/apache/pulsar/pull/14605 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Cancel offload tasks when managed ledger is closed.
 <br>https://github.com/apache/pulsar/pull/14545 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Tests] Fix the flaky test `AdminApiSchemaTest#testSchemaInfoApi`.
 <br>https://github.com/apache/pulsar/pull/14508 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Tests] Reduce memory usage im elastic container and clean up test cases.
 <br>https://github.com/apache/pulsar/pull/14580 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Tests] Fix the issue that `ManagedLedgerFactoryShutdownTest#openEncounteredShutdown` is flaky.
 <br>https://github.com/apache/pulsar/pull/14646 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Broker] Fix issues related to the deletion of namespaces.
 <br>https://github.com/apache/pulsar/pull/14657 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Fix the issue that the `HealthCheck` endpoint exposes race conditions.
 <br>https://github.com/apache/pulsar/pull/14618 
 <br>by [Technoboy-](https://github.com/Technoboy-)


### Ecosystem
- [OWASP] Upgrade mariadb-jdbc to 2.7.5 and add mariadb-jdbc to `owasp-dependency-check-suppressions.xml`.
 <br>https://github.com/apache/pulsar/pull/14593 
 <br>by [nodece](https://github.com/nodece)
- [Broker] Reduce memory usage in elastic container and clean up test cases.
 <br>https://github.com/apache/pulsar/pull/14631 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)


## Resources 
### Blog
- [Failure Is Not an Option; It Is a Given.](https://streamnative.io/blog/release/2022-03-07-failure-is-not-an-option-its-a-given/)
- [Pulsar, NiFi: Better Together for Messaging, Streaming](https://thenewstack.io/pulsar-nifi-better-together-for-messaging-streaming/)
- [Apache Pulsar Client Application Best Practices](https://streamnative.io/blog/engineering/2022-03-10-apache-pulsar-client-application-best-practices/)
- [Cloudera and StreamNative Announce the Integration of Apache NiFi™ and Apache Pulsar™](https://streamnative.io/blog/release/2022-03-09-cloudera-and-streamnative-announce-the-integration-of-apache-nifi-and-apache-pulsar/)

### Video
- [[Demo] Pulsar-NiFi Processor in Action](https://www.youtube.com/watch?v=LZG9IU6O78A)

## Release
- [Apache Pulsar Node.js client v1.6.2](https://github.com/apache/pulsar-client-node/releases)

## Events / News
- Past events
    - Virtual Meetup
        - [Apache Pulsar and Apache NiFi For Cloud Data Lakes](https://www.youtube.com/watch?v=2BeAQNI8Pu0)
    
- Upcoming events
    - 8 April, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - 17 May, 2022: Kubernetes Batch + HPC Day Europe
        - [Fast Data on-Ramp with Apache Pulsar on K8](https://kubernetesbatchdayeu22.sched.com/event/10F0q)
    - 18-20 July, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
