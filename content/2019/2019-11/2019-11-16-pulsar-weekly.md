---
title: "2019-11-16-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-11-09 ~ 2019-11-16"
date: 2019-11-09 ~ 2019-11-16
description: "This is the Pulsar community weekly update for 2019-11-09 ~ 2019-11-16, with updates on notable bug fixes around idempotent producer with external sequence id, data retention issues, features around java client and functions, and more."
id: "2019-11-16-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2019-11-09 ~ 2019-11-16

This is the Pulsar community weekly update for 2019-11-09 ~ 2019-11-16, with updates on notable bug fixes around idempotent producer with external sequence id, data retention issues, features around java client and functions, and more.

### Development

* [Release][Pulsar Manager] The 3rd candidate of Apache Pulsar Manager release 0.1.0 is out for voting.

    https://lists.apache.org/thread.html/3f48d6d3647cec1af5f4b70fbbeecb97f1a4df1166294c3cf012369b@%3Cdev.pulsar.apache.org%3E

* [Release][Pulsar] Xiaolong Ran started releasing 2.4.2.

    https://lists.apache.org/thread.html/511a0546c422fb353302b5252cf3fe7428885d29f8469564d9ff43b7@%3Cdev.pulsar.apache.org%3E
    
* [PIP-47] The community is voting to accept a time-based release plan.

    https://github.com/apache/pulsar/wiki/PIP-47%3A-Time-Based-Release-Plan

    https://lists.apache.org/thread.html/720580914b73ac7a4d8d915c07faee1d67d635e78aaf2d3583d26023@%3Cdev.pulsar.apache.org%3E

### Notable Feature

* [Client][Java] Expose include head message for durable consumers (Release: 2.4.3 / 2.5.0). 

    https://github.com/apache/pulsar/pull/5622
    
* [BookKeeper] Upgrade Apache BookKeeper version to 4.10.0 (Release: 2.4.2 / 2.5.0).

    https://github.com/apache/pulsar/pull/5607

* [Functions] Allow functions to pass runtime specific options (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5400
    
* [Client][Java] Introduce `batchingMaxBytes` setting in Pulsar producer (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5045

### Notable Bug Fix

* [Client][Java] Fix producer semaphore release error (Release: 2.4.2 / 2.5.0).

    https://github.com/apache/pulsar/pull/5587

* [Broker] Data is not deleted after expiration due to connected readers (Release: 2.4.2 / 2.5.0).

    https://github.com/apache/pulsar/pull/5621
    
* [Client] Fix message deduplicate issue while using external sequence id with batch produce (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5491
    
* [Broker][Metrics] Fix prometheus metrics export contains " bug (Release: 2.4.2 / 2.5.0).

    https://github.com/apache/pulsar/pull/5605

### Ecosystem

* [Client][DotNet] Pulsar.Client 0.10.0 released with API refinement.

    https://www.nuget.org/packages/Pulsar.Client/0.10.0
    
* [Client][DotNet] Pulsar.Client 0.9.0 released with support for key-based batching and concurrent consumer receive calls.

    https://www.nuget.org/packages/Pulsar.Client/0.9.1

### Event/News

* [Conference] Devoxx Morocco 2019 was held on November 12-14 in Agadir. Bruno Bonnin attended this conference and gave a talk about "Stream Processing with Apache Pulsar".

    https://twitter.com/ZenikaNantes/status/1194948501425274880
    
* [Meetup] A new Apache Pulsar meetup organized by Orange Financial and StreamNative was held on November 16 in Shanghai. Pulsar committers and contributors from Zhaopin, TuyaSmart, Orange Financial and StreamNative shared their experiences and best practices of running Pulsar on production.

    https://www.eventbrite.com/e/apache-pulsar-meetup-shanghai-tickets-79293658467

### Blog/Article

* How Orange Financial combats financial fraud over 50M transactions a day using Apache Pulsar (by Vincent Xie)

    https://streamnative.io/blog/tech/2019-11-11-how-orange-finaacial-combats-financial-fraud-over-50m-transactions-a-day-useing-apache-pulsar/

* Introduction to Apache Pulsar — Concepts, Architecture & Java Clients (by Florian Hussonnois)

    https://medium.com/streamthoughts/introduction-to-apache-pulsar-concepts-architecture-java-clients-71f1a30b75d6
