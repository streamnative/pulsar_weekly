---
title: "2021-08-23-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-08-16 ~ 2021-08-22"
date: 2021-08-16 ~ 2021-08-22
description: "This is the Pulsar community weekly update for 2021-08-16 ~ 2021-08-22, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-08-23-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-08-16 ~ 2021-08-22

This is the Pulsar community weekly update for 2021-08-16 ~ 2021-08-22, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[Technoboy-](https://github.com/Technoboy-), [gaoran10](https://github.com/gaoran10), [rdhabalia](https://github.com/rdhabalia), [315157973](https://github.com/315157973), [Anonymitaet](https://github.com/Anonymitaet), [wuzhanpeng](https://github.com/wuzhanpeng), [sanjivr](https://github.com/sanjivr), [Jason918](https://github.com/Jason918), [leizhiyuan](https://github.com/leizhiyuan), [JipeiWang](https://github.com/JipeiWang), [sijie](https://github.com/sijie), [tuteng](https://github.com/tuteng), [lhotari](https://github.com/lhotari), [sijia-w](https://github.com/sijia-w), [merlimat](https://github.com/merlimat), [wongxingjun](https://github.com/wongxingjun), [freeznet](https://github.com/freeznet), [abhilashmandaliya](https://github.com/abhilashmandaliya), [codelipenghui](https://github.com/codelipenghui), [bharanic-dev](https://github.com/bharanic-dev), [ivankelly](https://github.com/ivankelly), [Shoothzj](https://github.com/Shoothzj)


## Pulsar Program Overview
- Github Forks: 2.3k
- Github Stars: 9.5k
- Github Contributors: 439

## Pulsar Updates

### Notable Features

- [PIP 83] Allow Reader API to read and release pooled messages. 
<br>https://github.com/apache/pulsar/pull/11725 
<br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker] Remove subscription when closing Reader on non-persistent topics. 
<br>https://github.com/apache/pulsar/pull/11731 
<br>by [gaoran10](https://github.com/gaoran10)
- [Broker] Support disabling non-TLS service ports.
<br>https://github.com/apache/pulsar/pull/11681 
<br>by [lhotari](https://github.com/lhotari)
- [Admin] Avoid duplicate deletion of schema. 
<br>https://github.com/apache/pulsar/pull/11640 
<br>by [wuzhanpeng](https://github.com/wuzhanpeng)
- [Broker] Allow broker to start with default `backlogquota` in `byte`. 
<br>https://github.com/apache/pulsar/pull/11671 
<br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker] Add `shutdownGracefully` for `ManagedLedgerFactoryImpl`. 
<br>https://github.com/apache/pulsar/pull/11517 
<br>by [Jason918](https://github.com/Jason918)
 
### Notable Bug Fix

- [Broker] Fix the issue that cluster didn't respond error messages when throw `InterceptException`. 
<br>https://github.com/apache/pulsar/pull/11650 
<br>by [Technoboy-](https://github.com/Technoboy-)
- [Client] Set and return Topic-name in `Message::getTopicName()` API. 
<br>https://github.com/apache/pulsar/pull/11743 
<br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker] Pass the executor to RateLimiter in `ResourceGroupPublishLimiter`. 
<br>https://github.com/apache/pulsar/pull/11582 
<br>by [leizhiyuan](https://github.com/leizhiyuan)
- [C++] Fix the issue that broker pushes messages to consumer without restriction which causes memory issue in consumers. 
<br>https://github.com/apache/pulsar/pull/11692 
<br>by [merlimat](https://github.com/merlimat)
- [Client] Add Timeout to the list of "rejected"
responses. 
<br>https://github.com/apache/pulsar/pull/11688 
<br>by [ivankelly](https://github.com/ivankelly)

### Ecosystem

- [Pulsar IO] Pass client builder to debezium database history. 
<br>https://github.com/apache/pulsar/pull/11293 
<br>by [sijie](https://github.com/sijie)
- [Functions]Support protobuf schema. 
<br>https://github.com/apache/pulsar/pull/11709 
<br>by [tuteng](https://github.com/tuteng)
- [Admin] Allow user to create function with package URL through pulsar-admin. 
<br>https://github.com/apache/pulsar/pull/11666 
<br>by [freeznet](https://github.com/freeznet)
- [Functions] Fix the issue that terminateFunction does not clean up batch source intermediate topics which results in topic leak. 
<br>https://github.com/apache/pulsar/pull/11679 
<br>by [bharanic-dev](https://github.com/bharanic-dev)
 - [Python] Support `CryptoKeyReader` for Reader API in Python Clients. 
<br>https://github.com/apache/pulsar/pull/11447 
<br>by [sanjivr](https://github.com/sanjivr)


## Blog
- [Setup Producer & Consumer For Apache Pulsar Running On Docker](https://www.lionbloggertech.com/setup-producer-consumer-for-apache-pulsar-running-on-docker/)
- [5 More Reasons to Choose Apache Pulsar Over Apache Kafka](https://medium.com/building-the-open-data-stack/5-more-reasons-to-choose-apache-pulsar-over-apache-kafka-c09b259e3691)
- [Announcing Pulsar Summit Asia 2021: CFP Is Open!](https://streamnative.io/en/blog/community/pulsar-summit-asia-2021-cfp/)

## Events / News
- Upcoming Events
    - September 9th: [Webinar Series - Building Microservices with Pulsar](https://streamnative.zoom.us/webinar/register/WN_0vVCCqGhQ4G1978pZvxwZg)
    - September 16th: [Apache Pulsar Deep Dive, an end-to-end view of the data flow](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/280174947/)
    - September 21-23th: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)
- Call For Participation
    - [Pulsar Summit Asia 2021 CFP is Open](https://pulsar.apache.org/blog/2021/08/18/asia-cfp/)