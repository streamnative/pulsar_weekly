---
title: "2020-03-06-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-02-29 ~ 2020-03-06"
date: 2020-02-29 ~ 2020-03-06
description: "This is the Pulsar community weekly update for 2020-02-29 ~ 2020-03-06, with updates on introducing gPRC protocol handler on Pulsar broker, adding flags to disable auto creation of subscriptions, adding TenantAdmin interface to authorization, fixing multiple bugs for Pulsar 2.5.1, and so on."
---

## [Pulsar Community Weekly Update] 2020-02-29 ~ 2020-03-06

This is the Pulsar community weekly update for 2020-02-29 ~ 2020-03-06, with updates on introducing gPRC protocol handler on Pulsar broker, adding flags to disable auto creation of subscriptions, adding TenantAdmin interface to authorization, fixing multiple bugs for Pulsar 2.5.1, and so on.

### Development

- [PIP] A proposal is started to introduce a gRPC protocol handler for Pulsar.

    https://lists.apache.org/thread.html/r6937db21565a2c3fef00cfc3b19c611454c322631f16ddc38527e2fb%40%3Cdev.pulsar.apache.org%3E
    https://github.com/apache/pulsar/wiki/PIP-59%3A-gPRC-Protocol-Handler

### Notable Feature

- [Broker] Add configuration to disable auto creation of subscriptions (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6456
    
- [Broker] Enhance authorization by adding TenantAdmin interface (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6487

### Notable Bug Fix

- [Client][Java] Fix the logic of hasMessageAvailable (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6362
    
- [Client][Java] Fix the max backoff configuration for lookups (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6444
    
- [Broker] Fix memory leak when running topic compaction (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6485
    
- [Broker] Fix create a partitioned topic with a substring of an existing topic name (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6478
    
- [Schema] Each consumer should use different instances of schema (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6356

- [Broker] Create namespace failed when TLS is enabled in PulsarStandalone (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6457
    
### Event / News

- Trayan Iliev will give a talk about "Distributed Pub-Sub Messaging and Persistent Logging with Apache Pulsar" at Bulgarian Java Users Group on March 19.

    https://jug.bg/events/distributed-pub-sub-messaging-and-persistent-logging-with-apache-pulsar/
    