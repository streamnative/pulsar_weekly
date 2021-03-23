---
title: "2021-03-22-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-03-15 ~ 2021-03-21"
date: 2021-03-15 ~ 2021-03-21
description: "This is the Pulsar community weekly update for 2021-03-15 ~ 2021-03-21, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-03-22-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-03-15 ~ 2021-03-21

This is the Pulsar community weekly update for 2021-03-15 ~ 2021-03-21, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

Remove the direct ZooKeeper dependency from discovery-service and replace the ZooKeeper with the `MetadataStore`. Rename `ZookeeperCacheLoader` to `MetadataStoreCacheLoader` and use `MetadataStore` to access the ZooKeeper. This is one of the implementations of using `MetadataStore` API instead of the `ZookeeperCacheLoader`.

by ([@rdhabalia](https://github.com/rdhabalia))

### Notable Feature

- [Pulsar-Discovery] Replace ZooKeeper with `MetadataStore` in `discoveryservice`.

    https://github.com/apache/pulsar/pull/9967 ([@rdhabalia](https://github.com/rdhabalia))
    
- [Schema] Upgrade Apache Avro to version 1.10.2.

    https://github.com/apache/pulsar/pull/9898 ([@eolivelli](https://github.com/eolivelli))

- [Metrics] Add the broker connection metrics.

    https://github.com/apache/pulsar/pull/9876 ([@congbobo184](https://github.com/congbobo184))
    
- [Pulsar IO] The Kafka source connector supports managing Avro-encoded messages.

    https://github.com/apache/pulsar/pull/9448 ([@eolivelli](https://github.com/eolivelli))
    
- [Test] Add `TestNG` groups to the Pulsar broker.

    https://github.com/apache/pulsar/pull/9712 ([@aahmed-se](https://github.com/aahmed-se))

### Notable Bug Fix

- [Functions] Enable server-side routing for storing the state.

    https://github.com/apache/pulsar/pull/9978 ([@david-streamlio](https://github.com/david-streamlio))
    
- [Functions] Add `forwardSourceMessageProperty` to `SourceConfig`.

    https://github.com/apache/pulsar/pull/9945 ([@jerrypeng](https://github.com/jerrypeng))
    
- [Functions] Pass through record properties from Pulsar sources.

    https://github.com/apache/pulsar/pull/9943 ([@david-streamlio](https://github.com/david-streamlio))
    
- [CI] Fix the transaction flaky test.

    https://github.com/apache/pulsar/pull/9934 ([@congbobo184](https://github.com/congbobo184))
    
- [Functions] Add `forwardSourceMessageProperty` to `SourceConfig`.

    https://github.com/apache/pulsar/pull/9907 ([@freeznet](https://github.com/freeznet))
    
- [Broker] Fix the `zkBookieRackAffinityMapping` bug to support the BookKeeper `dnsResolver`.

    https://github.com/apache/pulsar/pull/9894 ([@hangc0276](https://github.com/hangc0276))
    
- [Broker] Fix the issue that non-persistent messages are not consumed in key_shared subscription mode.

    https://github.com/apache/pulsar/pull/9826 ([@MarvinCai](https://github.com/MarvinCai))

### Event / News

- [Webinar] Apache Flink x Pulsar Virtual Meetup: Streaming SQL at Uber and Facebook

    - Day One (03/16): https://www.youtube.com/watch?v=9ojajM7Zt0M&list=PLqRma1oIkcWgVbfmE0GDUkThnv_FNui7d&index=1
    - Day Two (03-17): https://www.youtube.com/watch?v=VcJ19mtsLNc&list=PLqRma1oIkcWgVbfmE0GDUkThnv_FNui7d&index=2

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- [Pulsar Office Hour] Monthly live stream about Pulsar best practices, use cases, and more.

  - 03/17: https://www.youtube.com/watch?v=ISjz_fHLR6w

### Blog / Article

- Announcing AWS SQS Connector for Apache Pulsar

    - https://streamnative.io/en/blog/tech/2021-03-17-announcing-aws-sqs-connector-for-apache-pulsar

