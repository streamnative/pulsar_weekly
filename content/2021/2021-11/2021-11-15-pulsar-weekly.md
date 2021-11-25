---
title: "2021-11-15-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-11-08 ~ 2021-11-14"
date: 2021-11-08 ~ 2021-11-14
description: "This is the Pulsar community weekly update for 2021-11-08 ~ 2021-11-14, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-11-15-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-11-08 ~ 2021-11-14

This is the Pulsar community weekly update for 2021-11-08 ~ 2021-11-14, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[Anonymitaet](https://github.com/Anonymitaet), [Shoothzj](https://github.com/Shoothzj), [michaeljmarshall](https://github.com/michaeljmarshall), [congbobo184](https://github.com/congbobo184), [yuruguo](https://github.com/yuruguo), [eolivelli](https://github.com/eolivelli), [Jason918](https://github.com/Jason918), [315157973](https://github.com/315157973), [nlu90](https://github.com/nlu90), [merlimat](https://github.com/merlimat), [gaozhangmin](https://github.com/gaozhangmin), [EronWright](https://github.com/EronWright), [rdhabalia](https://github.com/rdhabalia), [nicoloboschi](https://github.com/nicoloboschi), [Technoboy-](https://github.com/Technoboy-), [BewareMyPower](https://github.com/BewareMyPower), [urfreespace](https://github.com/urfreespace)
## Pulsar Program Overview
- Github Forks: 2.5k
- Github Stars: 10k
- Github Contributors: 465

## Pulsar Updates

### Highlights
- [Broker] Add support for namespace operation `UNSUBSCRIBE` when verifying the role's authorization.
<br>https://github.com/apache/pulsar/pull/12742 
<br>by [yuruguo](https://github.com/yuruguo)

- [Broker] Update Authentication interfaces to add a default implementation that calls `authenticate` method.
<br>https://github.com/apache/pulsar/pull/12104 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)


### Notable Features
- [Broker] Add support for namespace operation `UNSUBSCRIBE` when verifying the role's authorization.
<br>https://github.com/apache/pulsar/pull/12742 
<br>by [yuruguo](https://github.com/yuruguo)

- [Admin] Update command descriptions from old `property/cluster/namespace` format to current `tenant/namespace` format .
<br>https://github.com/apache/pulsar/pull/10485 
<br>by [eolivelli](https://github.com/eolivelli)


- [Broker] Expose broker bundles metrics to prometheus. 
<br>https://github.com/apache/pulsar/pull/12366 
<br>by [gaozhangmin](https://github.com/gaozhangmin)

- [Broker] Allow pulsar broker to lookup redirect for V1-topics with different clusters.
<br>https://github.com/apache/pulsar/pull/12743 
<br>by [rdhabalia](https://github.com/rdhabalia)
- [Broker] Add stop replicator producer logic in the `NamingException` when starting replicator cluster fails. 
<br>https://github.com/apache/pulsar/pull/12724 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [Broker] Apply `PolicyHierarchyValue` to `inactiveTopicPolicies` to avoid some complex checking on updates. 
<br>https://github.com/apache/pulsar/pull/12687 
<br>by [Jason918](https://github.com/Jason918)

### Notable Bug Fix
- [Broker] Fix the issue that `BookkeeperClientFactory` didn't pass in the ZooKeeper instance.
 <br>https://github.com/apache/pulsar/pull/12765 
 <br>by [EronWright](https://github.com/EronWright)
 
- [Broker] Update `ServerCnx` to close the connection after receiving unexpected `SendCommand`.
<br>https://github.com/apache/pulsar/pull/12780
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

- [Transaction] Fix the issue that broker or user can be created by transaction system topic.
<br>https://github.com/apache/pulsar/pull/12749 
<br>by [congbobo184](https://github.com/congbobo184)

- [Broker] Fix the issue that the `testDoNotReplicateSystemTopic` test method fails sporadically.
<br>https://github.com/apache/pulsar/pull/12775 
<br>by [Jason918](https://github.com/Jason918)

- [Transaction] Fix the issue that when `Transactionbuffersnapshot` topic is handling a null value， other topics recovered by which will produce NPE.
<br>https://github.com/apache/pulsar/pull/12758 
<br>by [congbobo184](https://github.com/congbobo184)

- [Metadata] Fix the logic error in `isValidPath`  and check the path before each operation in `AbstractMetadataStore`.
<br>https://github.com/apache/pulsar/pull/12663 
<br>by [Jason918](https://github.com/Jason918)

- [Broker] Fix the issue that consumers cannot be created although compatible is setted.
<br>https://github.com/apache/pulsar/pull/12721 
<br>by [315157973](https://github.com/315157973)

- [Client] Fix the issue that current implementation doesn't clean the file channel `os` even when `statusFuture` is complete.
<br>https://github.com/apache/pulsar/pull/12767 
<br>by [nlu90](https://github.com/nlu90)

 - [BookKeeper] Upgrade BookKeeper to 4.14.3.
<br>https://github.com/apache/pulsar/pull/12760 
<br>by [merlimat](https://github.com/merlimat)

- [Schema] Use Flaky Test to find the reason why `AdminApiSchemaTest#testSchemaInfoApi` failed. 
<br>https://github.com/apache/pulsar/pull/12461 
<br>by [nicoloboschi](https://github.com/nicoloboschi)

- [Admin] Fix `TestRunMain` test. 
<br>https://github.com/apache/pulsar/pull/12675 
<br>by [rdhabalia](https://github.com/rdhabalia)

- [Broker] Fix the issue that Flaky test was timed out.
<br>https://github.com/apache/pulsar/pull/12703 
<br>by [rdhabalia](https://github.com/rdhabalia)

- [BookKeeper] Fix the incorrect total size in `ManagedLedgerImpl` when `BrokerEntryMetadata` is enabled.
<br>https://github.com/apache/pulsar/pull/12714 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Admin] Reduce code duplication in Pulsar Admin classes. (Part2)
<br>https://github.com/apache/pulsar/pull/12748 
<br>by [eolivelli](https://github.com/eolivelli)

- [Broker] Allow to remove catching `NamingException` in `BrokerService#createNonPersistentTopic`.
<br>https://github.com/apache/pulsar/pull/12725 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [Admin] Reduce code duplication in Pulsar Admin classes. (Part1)
<br>https://github.com/apache/pulsar/pull/12732 
<br>by [eolivelli](https://github.com/eolivelli)

- [Broker] Remove unnecessary PowerMock annotation.
<br>https://github.com/apache/pulsar/pull/12713 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [Test] Test some depdency in integration tests scope.
<br>https://github.com/apache/pulsar/pull/12696 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [BookKeeper] Delete unused imports. 
<br>https://github.com/apache/pulsar/pull/12791 
<br>by [Shoothzj](https://github.com/Shoothzj)

## Resources
### Blog
- [Apache Pulsar: A Unified Queueing and Streaming Platform](https://thenewstack.io/apache-pulsar-a-unified-queueing-and-streaming-platform/)
- [Distributed Locks with Apache Pulsar](https://theboreddev.com/distributed-locks-with-apache-pulsar/)
- [Streaming Data Pipelines with Pulsar IO](https://streamnative.io/blog/engineering/2021-11-10-streaming-data-pipelines-with-pulsar-io/)
- [Event Streaming with Apache Pulsar and Scala](https://blog.rockthejvm.com/event-streaming-with-pulsar-and-scala/)
### Video
- [Apache Pulsar Tutorial with Scala](https://www.youtube.com/watch?v=u4lTUIFm1lw)

## Release 
- [Apache Pulsar Go Client 0.7](https://github.com/apache/pulsar-client-go/blob/master/CHANGELOG.md)

## Events / News
- Past Events
    - OSA CON 2021 – The Open Source Analytics Conference
        - [Hello Hydrate! From Stream to Clickhouse with Apache Pulsar and Friends](https://www.youtube.com/watch?v=K9MOiG1oz-0)
    
- Upcoming Events
    - December 3rd: Embedded Fest ONLINE
        - [Using Apache Pulsar to provide real-time analytics on the edge](https://embeddedfest.com/)