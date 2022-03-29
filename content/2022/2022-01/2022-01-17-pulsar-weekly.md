---
title: "2022-01-17-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-01-10 ~ 2022-01-16"
date: 2022-01-10 ~ 2022-01-16
description: "This is the Pulsar community weekly update for 2022-01-10 ~ 2022-01-16, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-01-17-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-01-10 ~ 2022-01-16

This is the Pulsar community weekly update for 2022-01-10 ~ 2022-01-16, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 


## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.6k
- Github Contributors: 513

## Pulsar Updates
### Highlights
- [Client] Add new TableView type and update the PulsarClient.
  <br>https://github.com/apache/pulsar/pull/12838 
  <br>by [nlu90](https://github.com/nlu90)
- [BookKeeper] Add system properties for the Bookie and BookieShell commands. 
  <br>https://github.com/apache/pulsar/pull/13296 
  <br>by [merlimat](https://github.com/merlimat)
- [Security] Upgrade Jackson to 2.12.6. 
  <br>https://github.com/apache/pulsar/pull/13694 
  <br>by [lhotari](https://github.com/lhotari)
- [Security] Upgrade protobuf to 3.16.1.
  <br>https://github.com/apache/pulsar/pull/13695 
  <br>by [lhotari](https://github.com/lhotari)
- [Security] Updated dependencies to get rid of pulsar-io/jdbc related CVE-2020-13692. 
  <br>https://github.com/apache/pulsar/pull/13753 
  <br>by [dlg99](https://github.com/dlg99)
- [Security] Added suppression for the CVE on Avro packages.
  <br>https://github.com/apache/pulsar/pull/13764 
  <br>by [nicoloboschi](https://github.com/nicoloboschi)

### Notable Features
- [Client] Add new TableView type and update the PulsarClient.
  <br>https://github.com/apache/pulsar/pull/12838 
  <br>by [nlu90](https://github.com/nlu90)
- [BookKepeper] Add system properties for the Bookie and BookieShell commands.
  <br>https://github.com/apache/pulsar/pull/13296 
  <br>by [merlimat](https://github.com/merlimat)
- [Broker] Offload policies support cross multiple clusters. 
  <br>https://github.com/apache/pulsar/pull/13534 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Support dynamic config for `replicationProducerQueueSize`. 
  <br>https://github.com/apache/pulsar/pull/13529 
  <br>by [lordcheng10](https://github.com/lordcheng10)

### Notable Bug Fix
- [BookKeeper] Fix the issue that invalid rack name prevents bookie from joining the rack. 
  <br>https://github.com/apache/pulsar/pull/13683 
  <br>by [hangc0276](https://github.com/hangc0276)
- [Broker] Fix the internal topic effect by `InactiveTopicPolicy`. 
  <br>https://github.com/apache/pulsar/pull/13611 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Fix the deadlock while using ZooKeeper thread to create ledger. 
  <br>https://github.com/apache/pulsar/pull/13744 
  <br>by [codelipenghui](https://github.com/codelipenghui)
- [Admin] Avoid call sync method in async rest API for delete subscription.
  <br>https://github.com/apache/pulsar/pull/13668 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Admin] Avoid call sync method in async rest API for delete subscription. 
  <br>https://github.com/apache/pulsar/pull/13666 
  <br>by [codelipenghui](https://github.com/codelipenghui)
- [Broker] Fix  the issue that `getInternalStats` occasionally lacks `LeaderInfo`. 
  <br>https://github.com/apache/pulsar/pull/13656 
  <br>by [shibd](https://github.com/shibd)
- [Client] Fix the Flaky-test `MultiTopicsReaderTest.testHasMessageAvailableAsync`.
  <br>https://github.com/apache/pulsar/pull/13634 
  <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Broker] Fix infinity values of CPU or Bandwidth usage .
  <br>https://github.com/apache/pulsar/pull/13609 
  <br>by [lordcheng10](https://github.com/lordcheng10)
- [Broker] When using the pulsar-aop test, add stack information when an exception is found.
  <br>https://github.com/apache/pulsar/pull/13553 
  <br>by [mingyifei](https://github.com/mingyifei)
- [Broker] Change ``ContextClassLoader`` to ``NarClassLoader`` in `BrokerInterceptor`. 
  <br>https://github.com/apache/pulsar/pull/13589 
  <br>by [mattisonchao](https://github.com/mattisonchao)
- [Broker] Fix the issue that no response to client because `PendingAckHandleImpl` init fail. 
  <br>https://github.com/apache/pulsar/pull/13655 
  <br>by [wenbingshen](https://github.com/wenbingshen)
- [Broker] Optimize `TopicPolicies#compactionThreshold` with `HierarchyTopicPolicies`. 
  <br>https://github.com/apache/pulsar/pull/13710 
  <br>by [AnonHxy](https://github.com/AnonHxy)


## Video
- [Build an Event-Driven Architecture with Pulsar](https://www.youtube.com/watch?v=mg7RLwV3x1M)
- [An Introduction to Transactions in Apache Pulsar](https://www.youtube.com/watch?v=OCBy1RZmTtU&t=26s)

## Events / News
- Survey
    - [[5-Min Survey] New Apache Pulsar Website](https://forms.office.com/pages/responsepage.aspx?id=DQSIkWdsW0yxEjajBLZtrQAAAAAAAAAAAAZAAOjIXw9UMFkzWUM0Q0JVSEtXWVY3SlM0UUMzQkxJVC4u)

- Upcoming events
    - March 30, 2022: Open Source Bristol
        - [Building a Scalable Event Streaming and Messaging Platform using Apache Pulsar for Fintech](https://www.meetup.com/Open-Source-Bristol/events/284198269/)
    - March 31, 2022: MLcof NYC
        - [Event-Driven Machine Learning at Scale](https://mlconf.com/speakers/timothy-spann/)
    - April 8, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - July 18-20, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html)
