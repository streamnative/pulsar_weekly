---
title: "2021-12-06-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-11-29 ~ 2021-12-05"
date: 2021-11-29 ~ 2021-12-05
description: "This is the Pulsar community weekly update for 2021-11-29 ~ 2021-12-05, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-12-06-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-11-29 ~ 2021-12-05

This is the Pulsar community weekly update for 2021-11-29 ~ 2021-12-05, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[Jason918](https://github.com/Jason918), [fantapsody](https://github.com/fantapsody), [merlimat](https://github.com/merlimat), [315157973](https://github.com/315157973), [Anonymitaet](https://github.com/Anonymitaet), [nlu90](https://github.com/nlu90), [lhotari](https://github.com/lhotari), [ericsyh](https://github.com/ericsyh), [Technoboy-](https://github.com/Technoboy-), [nicoloboschi](https://github.com/nicoloboschi), [hangc0276](https://github.com/hangc0276), [gaozhangmin](https://github.com/gaozhangmin), [dlg99](https://github.com/dlg99), [aloyszhang](https://github.com/aloyszhang), [MMirelli](https://github.com/MMirelli), [rdhabalia](https://github.com/rdhabalia), [michaeljmarshall](https://github.com/michaeljmarshall), [RocMarshal](https://github.com/RocMarshal), [sijia-w](https://github.com/sijia-w), [volgorean](https://github.com/volgorean)

## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.4k
- Github Contributors: 507

## Pulsar Updates
### Highlights
- [Broker]  Allow to configure metadata store URL in `broker.conf`.
 <br>https://github.com/apache/pulsar/pull/13077 
 <br>by [merlimat](https://github.com/merlimat)

### Notable Features
- [Broker] Add Metadata Store implemented with `RocksDataBase`.
 <br>https://github.com/apache/pulsar/pull/12776 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker]  Allow to configure metadata store URL in `broker.conf` .
 <br>https://github.com/apache/pulsar/pull/13077 
 <br>by [merlimat](https://github.com/merlimat)
- [Broker] Add pluggable entry filter in Dispatcher. 
 <br>https://github.com/apache/pulsar/pull/12970 
 <br>by [315157973](https://github.com/315157973)
- [Admin] Add the `--secrets` argument into `pulsar-admin [source|sink] create/update/localrun` command.
 <br>https://github.com/apache/pulsar/pull/13059 
 <br>by [nlu90](https://github.com/nlu90)
- [Client] Add `autorecovery` in Pulsar Cli. 
 <br>https://github.com/apache/pulsar/pull/13018 
 <br>by [ericsyh](https://github.com/ericsyh)
- [Broker] Use the `ZooKeeper.multi()` operation to do operations to ZK in batch.
 <br>https://github.com/apache/pulsar/pull/13043 
 <br>by [merlimat](https://github.com/merlimat)
- [Broker] Add `UniformLoadShedder` strategy to achieve goal for uniform load in cluster.
 <br>https://github.com/apache/pulsar/pull/12902 
 <br>by [rdhabalia](https://github.com/rdhabalia)
- [Java Client] Make `Audience` field optional in OAuth2 Client Credentials. 
 <br>https://github.com/apache/pulsar/pull/11988 
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)

### Notable Bug Fix
- [Broker] Don't attempt to delete pending ack store unless transactions are enabled. 
 <br>https://github.com/apache/pulsar/pull/13041 
 <br>by [lhotari](https://github.com/lhotari)
- [Pulsar Client] Use `sendAsync` instead of `send` when produce message to retry topic. 
 <br>https://github.com/apache/pulsar/pull/12946 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Fix the issue that unordered consuming case in Key_Shared subscription. 
 <br>https://github.com/apache/pulsar/pull/12890 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker] Fix the issue that metadata store is generating a lot of warning logs in unit test lately. 
 <br>https://github.com/apache/pulsar/pull/12896 
 <br>by [Jason918](https://github.com/Jason918)
- [BookKeeper] Delete the created ledger from broker cache and BookKeeper when updating ZNode list fails.
 <br>https://github.com/apache/pulsar/pull/12015 
 <br>by [hangc0276](https://github.com/hangc0276)
- [Pulsar IO] Move `AvroData` to a static final and remove unused fields.
 <br>https://github.com/apache/pulsar/pull/12859 
 <br>by [dlg99](https://github.com/dlg99)
- [Broker] Add a new field `revalidateFuture` to store the status of the last revalidate.
 <br>https://github.com/apache/pulsar/pull/13006 
 <br>by [Jason918](https://github.com/Jason918)
- [Broker] Add exec permissions to the Python Scripts in `/docker/pulsar/scripts`.
 <br>https://github.com/apache/pulsar/pull/11951 
 <br>by [MMirelli](https://github.com/MMirelli)
- [Broker] Fix `LeaderElectionService.getCurrentLeader` and add support for `empheralOwner` in MockZooKeeper.
 <br>https://github.com/apache/pulsar/pull/13117 
 <br>by [lhotari](https://github.com/lhotari)
- [Cleanup] Evaluate the current protocol version.
 <br>https://github.com/apache/pulsar/pull/13045 
 <br>by [lhotari](https://github.com/lhotari)
- [Functions] Fix the issue that some classloaders are leaked.
 <br>https://github.com/apache/pulsar/pull/12973 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Fix and improve topic ownership assignment. 
 <br>https://github.com/apache/pulsar/pull/13069 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Add new field `maxProducersPerTopic` to `org.apache.pulsar.broker.service.AbstractTopic#topicPolicies`.
 <br>https://github.com/apache/pulsar/pull/13082 
 <br>by [Jason918](https://github.com/Jason918)
- [Function]  Fix the issue that the metrics port is not exposed.
 <br>https://github.com/apache/pulsar/pull/12065 
 <br>by [volgorean](https://github.com/volgorean)

### Ecosystem
- [Pulsar IO] Use topic name as the index name if `indexName` is not configured.
 <br>https://github.com/apache/pulsar/pull/13064 
 <br>by [fantapsody](https://github.com/fantapsody)
- [Function] Fix the issue that the runtime of `instance-conf` is incorrect. 
 <br>https://github.com/apache/pulsar/pull/13031 
 <br>by [ericsyh](https://github.com/ericsyh)
- [Pulsar IO] Correct `@FieldDoc defaultValue` for some fields. 
 <br>https://github.com/apache/pulsar/pull/12697 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)

## Resources 
### Blog
- [Offset Implementation in Kafka-on-Pulsar](https://streamnative.io/blog/engineering/2021-12-01-offset-implementation-in-kafka-on-pulsar/)

### Slides
- [Using FLiP with InfluxDB for EdgeAI IoT at Scale](https://www.slideshare.net/bunkertor/using-flip-with-influxdb-for-edgeai-iot-at-scale-2022)
- [FLiP Into Apache Pulsar Apps with ScyllaDB](https://www.slideshare.net/bunkertor/streamnative-flip-into-scylladb-scylla-summit-2022)

## Events
- Upcoming events
    - March 10, 2022: FliPN Stack for Cloud Data Lakes | Meetup
        - [Using Apache Pulsar, Flink, and Nifi to Stream to Your Data Lakes](https://streamnative.io/en/event/meetup-flipn-stack-for-cloud-data-lakes/)
    - Philly ETE 2022
        - [Deep Dive Into Building Streaming Applications with Apache Pulsar](https://2022.phillyemergingtech.com/talks/deep-dive-into-building-streaming-applications-with-apache-pulsar/)
