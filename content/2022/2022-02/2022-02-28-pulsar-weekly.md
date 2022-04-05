---
title: "2022-02-28-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-02-21 ~ 2022-02-27"
date: 2022-02-21 ~ 2022-02-27
description: "This is the Pulsar community weekly update for 2022-02-21 ~ 2022-02-27, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-02-28-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-02-21 ~ 2022-02-27

This is the Pulsar community weekly update for 2022-02-21 ~ 2022-02-27, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[Shawyeok](https://github.com/Shawyeok), [gaozhangmin](https://github.com/gaozhangmin), [liangyepianzhou](https://github.com/liangyepianzhou), [Technoboy-](https://github.com/Technoboy-), [hangc0276](https://github.com/hangc0276), [BewareMyPower](https://github.com/BewareMyPower),  [codelipenghui](https://github.com/codelipenghui), [fantapsody](https://github.com/fantapsody), [ericsyh](https://github.com/ericsyh), [zdufour-asp](https://github.com/zdufour-asp), [tuteng](https://github.com/tuteng)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Highlights
- [Pulsar Client] Make `AbstractSchema#atSchemaVersion` throw an NPE only if `supportSchemaVersioning` is true and `schemaVersion` is null.
 <br>https://github.com/apache/pulsar/pull/14317 
 <br>by [Shawyeok](https://github.com/Shawyeok)

### Notable Features
- [Transaction] Adopt a single thread pool in  transaction coordinator.
 <br>https://github.com/apache/pulsar/pull/14238 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] Delete `changeMaxReadPositionAndAddAbortTimes` if `checkIfNoSnapshot() = true`.
 <br>https://github.com/apache/pulsar/pull/14276 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] Use `SingleThread` to handle TC-Client connecting.
 <br>https://github.com/apache/pulsar/pull/13969 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)


### Notable Bug Fix
- [Pulsar-Client] Make `AbstractSchema#atSchemaVersion` throw an NPE only if `supportSchemaVersioning` is true and `schemaVersion` is null.
 <br>https://github.com/apache/pulsar/pull/14317 
 <br>by [Shawyeok](https://github.com/Shawyeok)
- [Broker] Delete the cursor when consumer is closed.
 <br>https://github.com/apache/pulsar/pull/13939 
 <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Pulsar Admin] Delete `system topic` first and then delete `namespace bundles`.
 [Technoboy-](https://github.com/Technoboy-)
 <br>https://github.com/apache/pulsar/pull/14215 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Pulsar admin] Validate the rack name when setting the `bookie rack info`.
 <br>https://github.com/apache/pulsar/pull/14336 
 <br>by [hangc0276](https://github.com/hangc0276)
- [Transaction] Fix theissuethat end transaction in timeout state.
 <br>https://github.com/apache/pulsar/pull/14370 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Pulsar SQL] Fix the deserialization of `PulsarRecordCursor`.
 <br>https://github.com/apache/pulsar/pull/14379 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [C++ Client]  Add the `-Wno-stringop-truncation option` for `GCC >= 8.1`.
 <br>https://github.com/apache/pulsar/pull/14402 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Pulsar client] Call `.subscribeAsync` with `enableRetry(true)`.
 <br>https://github.com/apache/pulsar/pull/14433 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Fix the issue that the latest message on compacted topics could not be read.
 <br>https://github.com/apache/pulsar/pull/14449 
 <br>by [codelipenghui](https://github.com/codelipenghui)
- [Pulsar IO] Fix the issue that `pulsar-io-elasticsearch-sink1` supports rolling create index. 
 <br>https://github.com/apache/pulsar/pull/14383 
 <br>by [fantapsody](https://github.com/fantapsody)
- [Docs] Fix bare excepts in Python Client example code.
 <br>https://github.com/apache/pulsar/pull/14461 
 <br>by [zdufour-asp](https://github.com/zdufour-asp)
- [Docs] Fix the markdown format of the filesystem offloader document.
 <br>https://github.com/apache/pulsar/pull/14474 
 <br>by [ericsyh](https://github.com/ericsyh)
- [Broker] Fix the isuue that Pulsar cannot save and pass custom http auth status.
 <br>https://github.com/apache/pulsar/pull/14044 
 <br>by [tuteng](https://github.com/tuteng)

## Blog
- [Pulsar in Python on Pi for Sensors](https://dzone.com/articles/pulsar-in-python-on-pi)
- [Pulsar on KubeSphere: Installing Distributed Messaging and Streaming Platform](https://dzone.com/articles/pulsar-on-kubesphere-installing-distributed-messaging-and-streaming-platform)

## Release
- [SharePulsar v2.9.0](https://www.nuget.org/packages/SharpPulsar/2.9.0)
- [Apache Pulsar Go Client version v0.8.0](https://t.co/yHkVf8V6kg)

## Events / News
- Upcoming events
    - 8 April, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - 17 May, 2022: Kubernetes Batch + HPC Day Europe
        - [Fast Data on-Ramp with Apache Pulsar on K8](https://kubernetesbatchdayeu22.sched.com/event/10F0q)
    - 18-20 July, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
