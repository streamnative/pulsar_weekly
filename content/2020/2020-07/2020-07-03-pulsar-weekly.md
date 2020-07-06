---
title: "2020-07-03-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-06-27 ~ 2020-07-03"
date: 2020-06-27 ~ 2020-07-03
description: "This is the Pulsar community weekly update for 2020-06-27 ~ 2020-07-03, with updates on Pulsar.NET Client 1.4.2 release, a new feature (rebalance mechanism) implemented in Pulsar Functions, and so on."
id: "2020-07-03-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-06-27 ~ 2020-07-03

This is the Pulsar community weekly update for 2020-06-27 ~ 2020-07-03, with updates on Pulsar.NET Client 1.4.2 release, a new feature (rebalance mechanism) implemented in Pulsar Functions, and so on.

### Development

- [Release] Pulsar.NET Client 1.4.2 is released.

    https://www.nuget.org/packages/Pulsar.Client/1.4.2

### Notable Feature

- [Function] Implement rebalance mechanism in Pulsar Functions.

    https://github.com/apache/pulsar/pull/7388

- [Broker] After a bundle split, perform the unload in background.

    https://github.com/apache/pulsar/pull/7387
    
- [Java client] Support authentication with oauth2.

    https://github.com/apache/pulsar/pull/7420
    
- [Function] Improve security settings of Pulsar Functions.

    https://github.com/apache/pulsar/pull/7424
    
### Notable Bug Fix

- [Tiered storage] Fix NPE in GCS offloading operation.
    
    https://github.com/apache/pulsar/pull/7400
    
- [Broker] Fix producer stuck issue due to NPE thrown when creating a new ledger.

    https://github.com/apache/pulsar/pull/7401
    
- [Broker] Avoid NPE at ledger creation when DNS failures happen.

    https://github.com/apache/pulsar/pull/7403
    
- [Tiered storage] Shaded jclouds to avoid gson conflict.

    https://github.com/apache/pulsar/pull/7435

### Event / News

- [Pulsar Summit] The first-ever Pulsar Summit Virtual Conference 2020 was held on June 17 - 18. This two-day digital event featured more than 30 sessions from top Pulsar contributors and developers.

    All video recordings and slides are available at [here](https://streamnative.io/resource#pulsar-summit). 
    
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    All video recordings are available at [here](https://streamnative.io/resource#tgip). 

### Blog / Article

- Comparing Apache Kafka and Apache Pulsar - Jaroslaw Kijanowski

    https://blog.softwaremill.com/comparing-apache-kafka-and-apache-pulsar-3bd44e00f304
