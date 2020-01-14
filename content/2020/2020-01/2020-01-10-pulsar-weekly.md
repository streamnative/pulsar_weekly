---
title: "2020-01-10-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-01-04 ~ 2020-01-10"
date: 2020-01-04 ~ 2020-01-10
description: "This is the Pulsar community weekly update for 2020-01-04 ~ 2020-01-10, with updates on key-hash range reader and multiple critical bug fixes around broker and storage"
---

## [Pulsar Community Weekly Update] 2020-01-04 ~ 2020-01-10

This is the Pulsar community weekly update for 2020-01-04 ~ 2020-01-10, with updates on key-hash range reader and multiple critical bug fixes around broker and storage.

### Development

- [CI] After a bunch of fixes, the new CI based on GitHub Actions are stabilizing.

### Notable Feature

- [Avro] Upgrade Avro to 1.9.1 (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/5938
    
- [Broker] Prevent creation of regular topic with the same name as the existing partitioned topic (Release: 2.5.1).

    https://github.com/apache/pulsar/pull/5943
    
- [Broker] Fix create a consumer on partitioned topic while disable topic auto-creation (Release: 2.5.1).

    https://github.com/apache/pulsar/pull/5572
    
- [Java][Client] Add support for key hash range reading (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/5928

### Notable Bug Fix

- [Client][Java] Fix reader builder clone error (Release: 2.5.0, 2.4.3).

    https://github.com/apache/pulsar/pull/5923

- [Standalone] Make standalone to advertise "localhost" to avoid failure when a hostname is not resolvable (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5856
    
- [Broker] Close managed-ledgers before giving up bundle ownership to avoid bad zk-version (Release: 2.4.3).

    https://github.com/apache/pulsar/pull/5599
    
- [ML] Avoid using the same OpAddEntry between different ledger handles (Release: 2.5.1).

    https://github.com/apache/pulsar/pull/5942

### Event / News

- Apache IoTDB X Apache Pulsar meetup was held on Jan 4 in Beijing. Jia Zhai from StreamNative shared about "Apache Pulsar: from messaging system to event streaming platform". Besides, Guangning E from StreamNative gave a talk about "How to connect Apache Pulsar to IoTDB with Pulsar IO".

    https://www.eventbrite.com/e/apache-iotdb-x-apache-pulsar-meetup-tickets-85739618507#

