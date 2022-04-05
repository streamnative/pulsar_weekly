---
title: "2022-01-24-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-01-17 ~ 2022-01-23"
date: 2022-01-17 ~ 2022-01-23
description: "This is the Pulsar community weekly update for 2022-01-17 ~ 2022-01-23, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-01-24-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-01-17 ~ 2022-01-23

This is the Pulsar community weekly update for 2022-01-17 ~ 2022-01-23, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[freeznet](https://github.com/freeznet), [BewareMyPower](https://github.com/BewareMyPower), [gaozhangmin](https://github.com/gaozhangmin), [dlg99](https://github.com/dlg99), [mostafij-rahman](https://github.com/mostafij-rahman), [lhotari](https://github.com/lhotari), [RobertIndie](https://github.com/RobertIndie), [sijia-w](https://github.com/sijia-w), [liudezhi2098](https://github.com/liudezhi2098), [congbobo184](https://github.com/congbobo184), [Nicklee007](https://github.com/Nicklee007), [dragonls](https://github.com/dragonls), [Jason918](https://github.com/Jason918), [mattisonchao](https://github.com/mattisonchao), [Technoboy-](https://github.com/Technoboy-), [michaeljmarshall](https://github.com/michaeljmarshall), [merlimat](https://github.com/merlimat), [HQebupt](https://github.com/HQebupt), [nicoloboschi](https://github.com/nicoloboschi), [ofek](https://github.com/ofek), [aloyszhang](https://github.com/aloyszhang)

## Pulsar Program Overview
- Github Forks: 2.8k
- Github Stars: 10.6k
- Github Contributors: 514

## Pulsar Updates
### Highlights
- Add a new MetadataStore implementation based on etcd client.
 <br>https://github.com/apache/pulsar/pull/13225 
 <br>by [merlimat](https://github.com/merlimat)
 
### Notable Features
- [C++ Client] Support large message size. 
 <br>https://github.com/apache/pulsar/pull/13627 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Pulsar Client] PIP-120: Enable the `MemeoryLimitController`.
 <br>https://github.com/apache/pulsar/pull/13344 
 <br>by [HQebupt](https://github.com/HQebupt)
- [Broker] Add `configurationMetadataStore` to `PulsarClusterMetadataSetup`.
 <br>https://github.com/apache/pulsar/pull/13889 
 <br>by [RobertIndie](https://github.com/RobertIndie)
- [Broker] Return from the method early when policies are marked as read-only.
 <br>https://github.com/apache/pulsar/pull/12514 
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)

### Notable Bug Fix
- [Broker] Fix some potential NPE bug when get null value by Pulsar Admin.
 <br>https://github.com/apache/pulsar/pull/13831 
 <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Proxy] Fix the issue to prevent leak of unreleased `lookupRequestSemaphore` permits.
 <br>https://github.com/apache/pulsar/pull/13812 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Fix the issue that topics produced through REST do not support Authorization. 
 <br>https://github.com/apache/pulsar/pull/13771 
 <br>by [liudezhi2098](https://github.com/liudezhi2098)
- [Broker] Release old bundle from ownership cache when the operator splits  the old bundle. 
 <br>https://github.com/apache/pulsar/pull/13678 
 <br>by [Nicklee007](https://github.com/Nicklee007)
- [Broker] Add `isPersistent check` in `ServerCnx`.
 <br>https://github.com/apache/pulsar/pull/13685 
 <br>by [dragonls](https://github.com/dragonls)
- [Pulsar Client] Fix the issue that send chunking message failed when encryption is enabled.
 <br>https://github.com/apache/pulsar/pull/13689 
 <br>by [Jason918](https://github.com/Jason918)
- [Pulsar Client] Fix the issue that send chunking message failed when ordering key is set. 
 <br>https://github.com/apache/pulsar/pull/13699 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker] Fix call sync method in async rest API for `internalGetSubscriptionsForNonPartitionedTopic`. 
 <br>https://github.com/apache/pulsar/pull/13745 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- Fix managed cursor acknowledgment state metric names. 
 <br>https://github.com/apache/pulsar/pull/13844 
 <br>by [ofek](https://github.com/ofek)

### Ecosystem
- [Pulsar IO] Pass client builder if no service URL is provided to Debezium connector.
 <br>https://github.com/apache/pulsar/pull/12145 
 <br>by [freeznet](https://github.com/freeznet)

## Resources 
### Blog
- [Auto-Scaling Pulsar Functions in Kubernetes Using Custom Metrics](https://streamnative.io/blog/engineering/2022-01-19-auto-scaling-pulsar-functions-in-kubernetes-using-custom-metrics/)

### Slides
- [Apache Pulsar with MQTT for Edge Computing](https://www.slideshare.net/bunkertor/data-minutes-2-apache-pulsar-with-mqtt-for-edge-computing-lightning-2022)

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