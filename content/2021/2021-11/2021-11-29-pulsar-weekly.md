---
title: "2021-11-29-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-11-22 ~ 2021-11-28"
date: 2021-11-22 ~ 2021-11-28
description: "This is the Pulsar community weekly update for 2021-11-22 ~ 2021-11-28, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-11-29-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-11-22 ~ 2021-11-28

This is the Pulsar community weekly update for 2021-11-22 ~ 2021-11-28, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[codelipenghui](https://github.com/codelipenghui), [ericsyh](https://github.com/ericsyh), [Jason918](https://github.com/Jason918), [RobertIndie](https://github.com/RobertIndie), [lhotari](https://github.com/lhotari), [BewareMyPower](https://github.com/BewareMyPower), [nlu90](https://github.com/nlu90), [yuruguo](https://github.com/yuruguo), [michaeljmarshall](https://github.com/michaeljmarshall), [congbobo184](https://github.com/congbobo184), [massakam](https://github.com/massakam), [Anonymitaet](https://github.com/Anonymitaet), [urfreespace](https://github.com/urfreespace), [315157973](https://github.com/315157973), [gaozhangmin](https://github.com/gaozhangmin), [Technoboy-](https://github.com/Technoboy-)

## Pulsar Program Overview
- Github Forks: 2.5k
- Github Stars: 10k
- Github Contributors: 467

## Pulsar Updates

### Highlights
- [Broker] Support setting properties for subscriptions.
<br>https://github.com/apache/pulsar/pull/12869 
<br>by [315157973](https://github.com/315157973)
 
### Notable Features

- [Broker] Support setting properties for subscriptions.
<br>https://github.com/apache/pulsar/pull/12869 
<br>by [315157973](https://github.com/315157973)
 
### Notable Bug Fix

- [Broker] Disable recycle the `OpAddEntry` when the call to `OpAddEntry` fails. 
<br>https://github.com/apache/pulsar/pull/12993 
<br>by [codelipenghui](https://github.com/codelipenghui)
 
- [Broker] Avoid calling blocking metadata query in metadata-callback thread.
<br>https://github.com/apache/pulsar/pull/12753 
<br>by [Jason918](https://github.com/Jason918)
 
- [Broker] Fix NPE in `PersistentTopic.checkSubscriptionTypesEnable` .
<br>https://github.com/apache/pulsar/pull/12961 
<br>by [RobertIndie](https://github.com/RobertIndie)
 
- [Security] Use JDK default security provider when Conscrypt isn't available. 
<br>https://github.com/apache/pulsar/pull/12938 
<br>by [lhotari](https://github.com/lhotari)
 
- [Broker] Fix `ConcurrentOpenLongPairRangeSet#isEmpty`.
<br>https://github.com/apache/pulsar/pull/12953 
<br>by [BewareMyPower](https://github.com/BewareMyPower)
 
- [Broker] Fix the issue that the deletion topic method for `v1/topic` faces parameter loss and mismatch.
<br>https://github.com/apache/pulsar/pull/12936 
<br>by [yuruguo](https://github.com/yuruguo)
 
- [Broker]  Use `org.apache.pulsar.broker.service.TopicPoliciesService#unregisterListener` to remove unused listeners.
<br>https://github.com/apache/pulsar/pull/12904 
<br>by [Jason918](https://github.com/Jason918)
 
- [Broker] Add an async read topic policy and update procedure in `PersistentTopic#initialize`.
<br>https://github.com/apache/pulsar/pull/12833 
<br>by [Jason918](https://github.com/Jason918)

- [Broker] Delete `TopicPoliciesService#clean`. 
<br>https://github.com/apache/pulsar/pull/12913 
<br>by [Jason918](https://github.com/Jason918)
 
- [Broker] Support roles with consume namespace authorization `CLEAR_BACKLOG` subscriptions on a namespace.
<br>https://github.com/apache/pulsar/pull/12963 
<br>by [yuruguo](https://github.com/yuruguo)
 
- [Functions] Add `--secrets` argument into `pulsar-admin functions create/update/localrun` command.
<br>https://github.com/apache/pulsar/pull/12950 
 <br>by [nlu90](https://github.com/nlu90)
 
- [CLI] Support deploy autorecovery service seperately in Pulsar CLI. 
<br>https://github.com/apache/pulsar/pull/12985 
<br>by [ericsyh](https://github.com/ericsyh)

- [CI] Replace `adopt` with `temurin` in `actions/setup-java@v2`configuration.
<br>https://github.com/apache/pulsar/pull/12945 
<br>by [lhotari](https://github.com/lhotari)
 
- [Client] Avoid `IllegalStateException` in `ClientCnx` debug logs. 
<br>https://github.com/apache/pulsar/pull/12899 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)
 
- [Schema]  Fix the issue that Pulsar cannot decode data to `GenericRecord` when using Json or Avro primitive schema.
<br>https://github.com/apache/pulsar/pull/12886 
<br>by [congbobo184](https://github.com/congbobo184)
 
- [Client] Define and expose `PULSAR_VERSION` macro. 
<br>https://github.com/apache/pulsar/pull/12769 
<br>by [massakam](https://github.com/massakam)
 
- [Client] Fix incorrect table. 
<br>https://github.com/apache/pulsar/pull/12976 
<br>by [Anonymitaet](https://github.com/Anonymitaet)

 
- [Test] Fix flaky cases caused by message reception timeout in `testBlockBrokerDispatching`. 
<br>https://github.com/apache/pulsar/pull/12954 
<br>by [Jason918](https://github.com/Jason918)
 
- [Test] Move `ConsumerBatchReceiveTest` out of the quarantine test group. 
<br>https://github.com/apache/pulsar/pull/12992 
<br>by [codelipenghui](https://github.com/codelipenghui)
 
- [Test] Remove unused params in broker GC log.
<br>https://github.com/apache/pulsar/pull/11285 
<br>by [gaozhangmin](https://github.com/gaozhangmin)
 
- [Admin] Revert "Set default root log level to debug" and make `PULSAR_LOG_ROOT_LEVEL` default to `PULSAR_LOG_LEVEL`. 
<br>https://github.com/apache/pulsar/pull/12941 
<br>by [lhotari](https://github.com/lhotari)
 
- [Admin] Fix log level configuration for `pulsar-admin`, `pulsar-client` and `pulsar-perf`.
<br>https://github.com/apache/pulsar/pull/12915 
<br>by [lhotari](https://github.com/lhotari)

- [Broker] Clean up the metadata of the non-persistent partitioned topics. 
<br>https://github.com/apache/pulsar/pull/12910 
<br>by [Technoboy-](https://github.com/Technoboy-)
 
- [BookKeeper] Upgrade ZooKeeper from 3.5.7 to 3.5.9.
<br>https://github.com/apache/pulsar/pull/12981 
<br>by [lhotari](https://github.com/lhotari)
 
## Blog
- [10 Useful Pulsarctl Commands to Manage Your Cluster](https://streamnative.io/blog/engineering/2021-11-23-10-useful-pulsarctl-commands-to-manage-your-cluster/)
- [7 Reasons to Choose Apache Pulsar over Apache Kafka](https://www.thetechplatform.com/post/7-reasons-to-choose-apache-pulsar-over-apache-kafka)

## Releases
- [AWS Lambda Sink Version 2.7.0](https://hub.streamnative.io/connectors/lambda-sink/2.7.0/)


## Events / News
- Upcoming events
  - Embedded Fest ONLINE: [Using Apache Pulsar to provide real-time analytics on the edge](https://embeddedfest.com/)
  - [Virtual Book Launch: Apache Pulsar in Action](https://streamnative.io/event/webinar-book-launch/)
