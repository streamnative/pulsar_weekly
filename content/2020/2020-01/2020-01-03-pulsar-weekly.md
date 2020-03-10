---
title: "2020-01-03-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-12-21 ~ 2020-01-03"
date: 2019-12-21 ~ 2020-01-03
description: "This is the Pulsar community weekly update for 2019-12-21 ~ 2020-01-03, with updates on Pulsar Summit, Hacker news, and bug fixes for 2.5.0 release"
id: "2020-01-03-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2019-12-21 ~ 2020-01-03

This is the Pulsar community weekly update for 2019-12-21 ~ 2020-01-03, with updates on Pulsar Summit, Hacker news, and bug fixes for 2.5.0 release.

### Development

- [CI] Efforts are continued to make GitHub Actions stable enough so that we can move CI from ASF Jenkins to GitHub Actions.

- [Protocol Handler] A discussion thread about adding NSQ Protocol Support using the protocol handler framework.
  
    https://lists.apache.org/thread.html/9e2143af01f1c6e21046985f8f7d30fb6eab84b8993bd122cb5b72bc%40%3Cdev.pulsar.apache.org%3E
        
- [Pulsar Go Client] The development work for `pulsar-client-go` continues towards the first apache release.

### Notable Feature

- [Broker] Allow for namespace default of offload threshold (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5872

### Notable Bug Fix

- [Broker] Fix read 0 entries cause message stop dispatch (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5894
    
- [Stats] Fix wrong redelivery count while redeliver when consumer disconnected (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5895
    
- [Client][Java] Add SentConnectFrame state check when running `handleError` (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5913
    
- [Client][C++] Fix CPP client schema version (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5930
    
- [Proxy] Proxy doesn't use the right ca certificate to connect to brokers (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5971
    
- [Broker] ReadHandle.readAsync that does not catch the exception cause stalling consumption (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5965
    
- [Flink] Cache Pulsar client to make it shared among tasks in a process (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5900
    
- [Client][Reader] Fix reader builder clone error (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5923

### Ecosystem

- Pulsar.Client 0.12.0 released with delayed messages support.

    https://www.nuget.org/packages/Pulsar.Client/0.12.0

### Event / News

- The first Pulsar Summit will be held in April 2020 at San Francisco. The Call for Presentation and pre-registration are open.

    - Call for presentation: https://pulsar-summit.org/call-for-presentations/
    
    - Pre-registration: https://pulsar-summit.org/pre-registration/
    
- Pulsar ranked 1st in Hacker News on Jan 2. Many engineers talked about "Why chooses Pulsar over Kafka, RabbitMQ, Kinesis or other MQ", "Pulsar features", and other topics.

    https://news.ycombinator.com/item?id=21936252

### Blog / Article

- From Apache Spark connector to Apache Pulsar basic concepts (by Bartosz Konieczny)

    https://www.waitingforcode.com/apache-pulsar/from-apache-spark-connector-to-apache-pulsar-basic-concepts/read
