---
title: "2022-02-14-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-02-07 ~ 2022-02-13"
date: 2022-02-07 ~ 2022-02-13
description: "This is the Pulsar community weekly update for 2022-02-07 ~ 2022-02-13, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-02-14-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-02-07 ~ 2022-02-13

This is the Pulsar community weekly update for 2022-02-07 ~ 2022-02-13, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[lhotari](https://github.com/lhotari), [fanjianye](https://github.com/fanjianye), [gaoran10](https://github.com/gaoran10), [merlimat](https://github.com/merlimat), [congbobo184](https://github.com/congbobo184), [michaeljmarshall](https://github.com/michaeljmarshall), [liangyepianzhou](https://github.com/liangyepianzhou), [RobertIndie](https://github.com/RobertIndie), [Jason918](https://github.com/Jason918), [nicoloboschi](https://github.com/nicoloboschi), [codelipenghui](https://github.com/codelipenghui), [callumduffy](https://github.com/callumduffy), [mattisonchao](https://github.com/mattisonchao), [Technoboy-](https://github.com/Technoboy-), [gaozhangmin](https://github.com/gaozhangmin), [ZiyaoWei](https://github.com/ZiyaoWei), [wangzhiwubigdata](https://github.com/wangzhiwubigdata), [freeznet](https://github.com/freeznet), [aloyszhang](https://github.com/aloyszhang)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Notable Bug Fix
- [Metadata] Let entries expire in the metadata caches 
 <br>https://github.com/apache/pulsar/pull/14154 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Remove the semaphore at the end of transactions operations.
 <br>https://github.com/apache/pulsar/pull/14131 
 <br>by [merlimat](https://github.com/merlimat)
- [Security] Upgrade both `jdbc` and `debezium` Postgre java driver dependency to 42.2.25.
 <br>https://github.com/apache/pulsar/pull/14119 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Pulsar client] Fix the race condition of `OpSendMsgQueue` when posting messages. 
 <br>https://github.com/apache/pulsar/pull/14231 
 <br>by [codelipenghui](https://github.com/codelipenghui)


## Resources 
### Blog
- [Multi-Tenancy Systems: Apache Pulsar vs. Kafka](https://datastax.medium.com/multi-tenancy-systems-apache-pulsar-vs-kafka-5442c9916da8)

### Video
- [Apache Pulsar integration (Microservices with .NET 6.0) episode #9](https://www.youtube.com/watch?v=WB72UGqTDoY)

## Events / News
- Upcoming events
    - 8 April, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - 17 May, 2022: Kubernetes Batch + HPC Day Europe
        - [Fast Data on-Ramp with Apache Pulsar on K8](https://kubernetesbatchdayeu22.sched.com/event/10F0q)
    - 18-20 July, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
