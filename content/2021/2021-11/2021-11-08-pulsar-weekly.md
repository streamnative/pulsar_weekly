---
title: "2021-11-08-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-11-01 ~ 2021-11-07"
date: 2021-11-01 ~ 2021-11-07
description: "This is the Pulsar community weekly update for 2021-11-01 ~ 2021-11-07, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-11-08-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-11-01 ~ 2021-11-07

This is the Pulsar community weekly update for 2021-11-01 ~ 2021-11-07, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[hanmz](https://github.com/hanmz), [RobertIndie](https://github.com/RobertIndie), [gaoran10](https://github.com/gaoran10), [thomasleplus](https://github.com/thomasleplus), [codelipenghui](https://github.com/codelipenghui), [merlimat](https://github.com/merlimat), [lhotari](https://github.com/lhotari), [Shoothzj](https://github.com/Shoothzj), [dlg99](https://github.com/dlg99), [massakam](https://github.com/massakam), [yuruguo](https://github.com/yuruguo), [tomscut](https://github.com/tomscut), [eolivelli](https://github.com/eolivelli), [Technoboy-](https://github.com/Technoboy-), [junqingzh](https://github.com/junqingzh), [baomingyu](https://github.com/baomingyu), [315157973](https://github.com/315157973), [Jason918](https://github.com/Jason918), [Demogorgon314](https://github.com/Demogorgon314), [x-shadow-man](https://github.com/x-shadow-man), [hangc0276](https://github.com/hangc0276)

## Pulsar Program Overview
- Github Forks: 2.5k
- Github Stars: 9.9k
- Github Contributors: 464

## Pulsar Updates

### Highlights
- [Broker] Add negative ACK redelivery backoff.
<br>https://github.com/apache/pulsar/pull/12566 
<br>by [hanmz](https://github.com/hanmz)
- [Broker] Fix call sync method in an async callback when enabling GEO replicator.
<br>https://github.com/apache/pulsar/pull/12590
<br>by [codelipenghui](https://github.com/codelipenghui)

### Notable Features
- [Broker] Support setting geo-replication clusters on topic level. 
<br>https://github.com/apache/pulsar/pull/12136
<br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Support retry when creating reader of topic policies. 
<br>https://github.com/apache/pulsar/pull/12622
<br>by [315157973](https://github.com/315157973)

### Notable Bug Fix
- [Broker] Fix prefix setting in JWT authentication and avoid multi calls for the `getProperty`. 
<br>https://github.com/apache/pulsar/pull/12132
<br>by [RobertIndie](https://github.com/RobertIndie)
- [Admin]: Fix last exit code storage. 
<br>https://github.com/apache/pulsar/pull/12581
<br>by [thomasleplus](https://github.com/thomasleplus)
- [Broker] Fix false positive ownership check in `OwnershipCache#checkOwnership`. 
<br>https://github.com/apache/pulsar/pull/12650
<br>by [Jason918](https://github.com/Jason918)
- [BookKeeper] Avoid passing `OpAddEntry` across a thread boundary in `asyncAddEntry`. 
<br>https://github.com/apache/pulsar/pull/12606
<br>by [lhotari](https://github.com/lhotari)
- [BookKeeper] Avoid move the non-durable cursor position when reading the compacted data.
<br>https://github.com/apache/pulsar/pull/12602 
<br>by [codelipenghui](https://github.com/codelipenghui)
- [Client] Fix the issue that `StartMessageId` and `RollbackDuration` don't work in `MultiTopicsReader` for non-partitioned topics. 
<br>https://github.com/apache/pulsar/pull/12308
<br>by [Jason918](https://github.com/Jason918)
- [Broker] Fix the issue that additional servlets NAR might extract to null directory.
<br>https://github.com/apache/pulsar/pull/12585 
<br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Broker] Fix cherry-pick code style.
<br>https://github.com/apache/pulsar/pull/12627
<br>by [hangc0276](https://github.com/hangc0276)

### Ecosystem
- [Schema] Support custom Avro configurations for Enum type on Python schema. 
<br>https://github.com/apache/pulsar/pull/12642
<br>by [gaoran10](https://github.com/gaoran10)
- [Functions] Allow to configure different implementations for Pulsar Functions state store. 
<br>https://github.com/apache/pulsar/pull/12646
<br>by [merlimat](https://github.com/merlimat)
- [Functions] Force deletion to avoid hung function worker during connector restart on K8s runtime. 
<br>https://github.com/apache/pulsar/pull/12504
<br> by [dlg99](https://github.com/dlg99)


## Resources

### Blog
- [Article] [Why Pulsar Beats Kafka for a Scalable, Distributed Data Architecture](https://jaxenter.com/pulsar-kafka-175830.html)
- Osacon 2021 
    - [Slides] [Hello Hydrate! From Stream to Clickhouse with Apache Pulsar and Friends](https://www.slideshare.net/bunkertor/osacon-2021-hello-hydrate-from-stream-to-clickhouse-with-apache-pulsar-and-friends) by. Timothy Spann

### Video
- Flink Forward Global 2021
  - [Interactive Session: AMA | Pulsar and Flink for Unified Data Processing](https://www.youtube.com/watch?v=sl1d7vZYe1E)

## Events / News
- Past Events
   - November 2nd-3rd: OSA Con 2021 | Open Source & Analytics Conference
        - [Hello Hydrate! From Stream to ClickHouse with Apache Pulsar and Friends](https://www.youtube.com/watch?v=K9MOiG1oz-0) by. Timothy Spann
- Upcoming Events
    - November 18th: [Conference - DeveloperWeek Austin](https://www.developerweek.com/Austin/conference/)
        - Deploying Machine Learning Models with Pulsar Functions
    - December 3rd: [Embedded Fest ONLINE](https://embeddedfest.com/)
