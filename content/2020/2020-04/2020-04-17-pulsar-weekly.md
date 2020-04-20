---
title: "2020-04-17-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-04-04 ~ 2020-04-17"
date: 2020-04-04 ~ 2020-04-17
description: "This is the Pulsar community weekly update for 2020-04-04 ~ 2020-04-17, with updates on multiple PIPs around schema, security, performance, and official Pulsar Helm chart support."
id: "2020-04-17-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-04-04 ~ 2020-04-17

This is the Pulsar community weekly update for 2020-04-04 ~ 2020-04-17, with updates on multiple PIPs around schema, security, performance, and official Pulsar Helm chart support.

### Development

- [Release] The fourth release candidate of Pulsar 2.5.1 is out for voting.

    https://lists.apache.org/thread.html/r0c1bb3c35d5bba326599e12e5fd3d2bb4830ebfcdd736d4f270640a7%40%3Cdev.pulsar.apache.org%3E
    
- [PIP-62] Move connectors, adapters, and presto connector to separate repositories.

    https://lists.apache.org/thread.html/r957c29cba3879cb7e46bd2fa4bc8d9602f20f10a5840e74a43f02d39%40%3Cdev.pulsar.apache.org%3E
    https://github.com/apache/pulsar/wiki/PIP-62:-Move-connectors,-adapters-and-Pulsar-Presto-to-separate-repositories
    
- [Pulsar Helm Chart] Pulsar Helm Chart is updated with many enhancements. The official Helm chart will be moved to a separate [chart repo](https://github.com/apache/pulsar-helm-chart) as a part of PIP-62.
  
    - Get started: https://pulsar.apache.org/docs/en/kubernetes-helm/
  
    - Documentation: https://pulsar.apache.org/docs/en/helm-overview/

### Notable Features

- [PIP-58] Support Consumers Set Custom Retry Delay (Release: 2.6.0).

    https://github.com/apache/pulsar/wiki/PIP-58-%3A-Support-Consumers--Set-Custom-Retry-Delay
    https://github.com/apache/pulsar/pull/6449
    
- [Schema] Add Joda time logical type conversion (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6704
    
- [Broker] Implement AutoSubscriptionCreation by namespace override (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6637
    
- [Security] Add audience verify in AuthenticationProviderToken (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6716

### Notable Bug Fix

- Issue-6612: Parse long field in GenericJsonRecord (Release: 2.5.2, 2.6.0).

    https://github.com/apache/pulsar/pull/6622
    
- Issue-6676: Retention policy should be respected when there is no traffic (Release: 2.5.2, 2.6.0).

    https://github.com/apache/pulsar/pull/6676
    
- Issue-6650: Fix send get raw schema request (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6650
    
- Issue-6685: Not allow sub auto create by admin when disable topic auto create (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6685
    
- Issue-6683: [Broker] Handle BadVersionException thrown by updateSchemaLocator() (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6683
    
- Issue-6695: [AVRO ENCODE] Reset cursor if message encode fails (Release: 2.5.2, 2.6.0).

    https://github.com/apache/pulsar/pull/6695


### Ecosystem

- [BookKeeper] Bookkeeper Visual Manager 1.0.0 is released. This application allows you to easily connect to your Bookkeeper, check the health of bookies, view and filter ledgers, check the cluster-wide configurations, and so on.

    https://github.com/diennea/bookkeeper-visual-manager

### Event / News

- TGI Pulsar (#TGIP): weekly live stream about Pulsar and its ecosystem
  
    - 005: Take a deep-dive into Pulsar architecture for performance tuning
  
        - Recording: https://www.youtube.com/watch?v=8O_RNYHX9tI
  
    - 006: Lifecycle of a Pulsar message
  
        - Recording: https://www.youtube.com/watch?v=R197TYYFaiI

- Upcoming events
  
    - 04/28: StreamNative Webinar - "Common architectural patterns on Apache Pulsar" by Devin Bost
  
        - Registration link: https://zoom.us/webinar/register/7515867672387/WN_eV-yBB-aQ0yU4uqLvPpgjg 
        
    - 04/30: "Event Streaming with Apache Pulsar" by Sijie Guo in open source community data #ossday
  
        - Registration link: https://web.cvent.com/event/001916f7-391a-4e9e-b0d8-0688882c85e3/summary?RefId=Web

### Blog / Article

- Taking a Deep-Dive into Apache Pulsar Architecture for Performance Tuning (by Devin Bost and Penghui Li)

    https://streamnative.io/whitepaper/taking-a-deep-dive-into-apache-pulsar-architecture-for-performance-tuning/

- 4 Data Trends to Watch in 2020 (by Astasia Myers)

    https://medium.com/memory-leak/4-data-trends-to-watch-in-2020-491707902c09

- How to Build a Distributed Database with Apache BookKeeper — Part 2 (by Enrico Olivelli)

    https://streamnative.io/blog/tech/2020-04-14-distributed-database-bk2/