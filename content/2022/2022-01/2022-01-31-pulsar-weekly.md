---
title: "2022-01-31-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-01-24 ~ 2022-01-30"
date: 2022-01-24 ~ 2022-01-30
description: "This is the Pulsar community weekly update for 2022-01-24 ~ 2022-01-30, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-01-31-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-01-24 ~ 2022-01-30

This is the Pulsar community weekly update for 2022-01-24 ~ 2022-01-30, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[nodece](https://github.com/nodece), [Technoboy-](https://github.com/Technoboy-), [addisonj](https://github.com/addisonj), [congbobo184](https://github.com/congbobo184), [lhotari](https://github.com/lhotari), [eolivelli](https://github.com/eolivelli), [hangc0276](https://github.com/hangc0276), [liangyepianzhou](https://github.com/liangyepianzhou), [Jason918](https://github.com/Jason918), [HQebupt](https://github.com/HQebupt), [gaozhangmin](https://github.com/gaozhangmin), [yuruguo](https://github.com/yuruguo), [liudezhi2098](https://github.com/liudezhi2098), [codelipenghui](https://github.com/codelipenghui), [rdhabalia](https://github.com/rdhabalia), [merlimat](https://github.com/merlimat), [mattisonchao](https://github.com/mattisonchao), [suiyuzeng](https://github.com/suiyuzeng)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Notable Features
- [BookKeeper] Support Topic metadata create topics with properties. 
 <br>https://github.com/apache/pulsar/pull/12818 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Proxy] Allow IO and acceptor threads to be configured in the proxy. 
 <br>https://github.com/apache/pulsar/pull/14054 
 <br>by [addisonj](https://github.com/addisonj)
- [Function] Allow metadata store URL to be configured `in functions_worker.yml`. 
 <br>https://github.com/apache/pulsar/pull/13782 
 <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Pulsar Client] PIP-121: Add Pulsar cluster level auto failover.
 <br>https://github.com/apache/pulsar/pull/13316
 <br>by [hangc0276](https://github.com/hangc0276)

 
### Notable Bug Fix
- [Broker] Fix the prioritization of read schema compatibility strategy.
 <br>https://github.com/apache/pulsar/pull/13938 
 <br>by [nodece](https://github.com/nodece)
- [Broker] Add `judge Subscription.isIndividualAckMode(subType)` when get `ackCount`.
 <br>https://github.com/apache/pulsar/pull/14021 
 <br>by [congbobo184](https://github.com/congbobo184)
- [Broker] Decrease `unackedMessages` count when call `individualAckNormal`.
 <br>https://github.com/apache/pulsar/pull/13383 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Add the entry to the list of messaged to be redelivered.
 <br>https://github.com/apache/pulsar/pull/14014 
 <br>by [eolivelli](https://github.com/eolivelli)
- [Schema] Skip add the DecimalConversion in `extractAvroSchema()`.
 <br>https://github.com/apache/pulsar/pull/14019 
 <br>by [nodece](https://github.com/nodece)
- [Test] Trim the value string on `PulsarConfigurationLoader` load process.
 <br>https://github.com/apache/pulsar/pull/13984 
 <br>by [hangc0276](https://github.com/hangc0276)
- [Transaction] Fix the individual ack with transaction decrease `unAckMessageCounnt`. 
 <br>https://github.com/apache/pulsar/pull/14020 
 <br>by [congbobo184](https://github.com/congbobo184)
- [Transaction] Fix the isseu that `RetryException` should not be return. 
 <br>https://github.com/apache/pulsar/pull/13828 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] `PendingAckHandleImpl` handle `isInCacheRequest`. 
 <br>https://github.com/apache/pulsar/pull/13481 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Broker] Clean up active consumer on connection that was already closed.
 <br>https://github.com/apache/pulsar/pull/13196 
 <br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker] Fix the issue that Consumer cannot consume messages when `key_shared` mode is configured as `subscriptionKeySharedUseConsistentHashing`.
 <br>https://github.com/apache/pulsar/pull/13991 
 <br>by [merlimat](https://github.com/merlimat)

## Resources 
### Blog
- [Moving Toward a ZooKeeper-Less Apache Pulsar](https://streamnative.io/blog/release/2022-01-25-moving-toward-a-zookeeperless-apache-pulsar/)
- [Streaming Analytics with Apache Pulsar and Spark Structured Streaming](https://blog.rockthejvm.com/pulsar-spark/)

### Video
- [Apache Pulsar with MQTT for Edge Computing](https://www.youtube.com/watch?v=sPGyl6XgGHw)
- [DevFest UKI 2021 - Hot Tech (Track 01)](https://www.youtube.com/watch?v=RZrnGHRYdks&t=12817s)

### Slides
- [Using Apache NiFi with Apache Pulsar for FRast Data On-Ramp](https://www.slideshare.net/bunkertor/devfest-uk-ireland-using-apache-nifi-with-apache-pulsar-for-fast-data-onramp-2022)


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