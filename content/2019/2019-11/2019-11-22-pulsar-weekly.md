---
title: "2019-11-22-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-11-17 ~ 2019-11-22"
date: 2019-11-17 ~ 2019-11-22
description: "This is the Pulsar community weekly update for 2019-11-17 ~ 2019-11-22, with updates on multiple under-voting Pulsar releases, support CDC connector for MongoDB, support batch receive in Java client, and more."
---

## [Pulsar Community Weekly Update] 2019-11-17 ~ 2019-11-22

This is the Pulsar community weekly update for 2019-11-17 ~ 2019-11-22, with updates on multiple under-voting Pulsar releases, support CDC connector for MongoDB, support batch receive in Java client, and more.

### Development

- [Release][Pulsar] RC1 for Apache Pulsar release 2.4.2 is out of voting.

    https://lists.apache.org/thread.html/81a702b1a45724657fba7298f0e4f51b32b60d0d10868e8423b12f62@%3Cdev.pulsar.apache.org%3E

- [Release][Pulsar Manager] RC4 for Pulsar Manager Release 0.1.0 is out for voting.

    https://lists.apache.org/thread.html/daf65d184d1a99336753b8c548714ca884705216ded090db145f3388@%3Cdev.pulsar.apache.org%3E
    
- [Release][Pulsar] Sijie started the discussion of cutting the Pulsar 2.5.0 release next week.

    https://lists.apache.org/thread.html/2135d54d33eee35ca7f8db927185bef0c57f98d9f9ea267d36fbca14@%3Cdev.pulsar.apache.org%3E

- [Pulsar Manager] Guangning started the initiative of adding authentication and authorization support in Pulsar Manager.

    https://lists.apache.org/thread.html/e7889faf0686875c7a0471afb4acd37342348b9f1393806776d92339@%3Cdev.pulsar.apache.org%3E

- [PIP-38] Support batch receive in Java client (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/4621
    
    https://github.com/apache/pulsar/wiki/PIP-38%3A-Batch-Receiving-Message

### Notable Feature

- [Connector] Support CDC connector for MongoDB (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5590
    
- [Functions] Parametrize grpc and metrics ports so that they can be configured (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5674
    
- [Broker][Stats] Expose lastExpireTimestamp for subscription stats. (Release: 2.4.3, 2.5.0).

    https://github.com/apache/pulsar/pull/5721

### Notable Bug Fix

- [Client][Java] Fix "Producer with name xyz is already connected to topic" (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5571
    
- [Client][Java] `hasMessageAvailable` should return false when Reader read from latest messages (Release: 2.4.3, 2.5.0).

    https://github.com/apache/pulsar/pull/5023
    
- [Client][Python] Fix Python consumer receive always timeout after 100ms (Release: 2.4.3, 2.5.0).

    https://github.com/apache/pulsar/pull/5706

### Event/News

* [Conference] KubeCon + CloudNativeCon North America 2019 was held on November 18-21 in San Diego. Yahoo! JAPAN was one of the gold sponsors. Pulsar team and Athenz team from Yahoo! JAPAN attended the conference as the booth exhibitor.

    https://twitter.com/Jennife06125739/status/1197930239646732295
    
    https://events19.linuxfoundation.org/events/kubecon-cloudnativecon-north-america-2019/sponsor/

* Pulsar Slack channel has more than 1250 users, which is momentum behind Pulsar community growth.

    https://twitter.com/streamnativeio/status/1197576910915506176
