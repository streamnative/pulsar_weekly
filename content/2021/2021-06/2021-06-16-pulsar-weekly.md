---
title: "2021-06-16-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-06-07 ~ 2021-06-13"
date: 2021-06-07 ~ 2021-06-13
description: "This is the Pulsar community weekly update for 2021-06-07 ~ 2021-06-13, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-06-16-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-06-07 ~ 2021-06-13

This is the Pulsar community weekly update for 2021-06-07 ~ 2021-06-13, with updates on Pulsar client, broker, transactions, and so on.

### Development

- [Client] Make `KeyValueSchema` as an interface available in the public Schema API.

    https://github.com/apache/pulsar/pull/10888 ([@eolivelli](https://github.com/eolivelli))

- [Metadata] Ensure that the metadata cache consistent across brokers.

    https://github.com/apache/pulsar/pull/10862 ([@sursingh](https://github.com/sursingh))

- [Broker] Optimize the prompt message when no topic exists.

    https://github.com/apache/pulsar/pull/10845 ([@315157973](https://github.com/315157973))

### Notable Feature

- [Broker] Introduce the `metricsServletTimeoutMs` setting.

    https://github.com/apache/pulsar/pull/10886 ([@sijie](https://github.com/sijie))

### Notable Bug Fix

- [C++] Fix the undefined behavior caused by uninitialized variables.

    https://github.com/apache/pulsar/pull/10892 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Broker] Fix improper `class/method/field` modifiers.

    https://github.com/apache/pulsar/pull/10837 ([@hangc0276](https://github.com/hangc0276))

- [Broker] Support automatically creating the system topic `TRANSACTION_BUFFER_SNAPSHOT`.

    https://github.com/apache/pulsar/pull/10876  ([@michaeljmarshall](https://github.com/michaeljmarshall))

- [Client] Remove the unwanted dependencies in the Pulsar Functions' instance JARs and make `SchemaInfo` as an interface.

    https://github.com/apache/pulsar/pull/10878  ([@jerrypeng](https://github.com/jerrypeng))

### Ecosystem

- [Connector] Kafka sink connector supports the non-primitive schema.

    https://github.com/apache/pulsar/pull/10410  ([@dlg99](https://github.com/dlg99))

- [Connector] Load credentials from secrets for Kinesis connectors.

    https://github.com/apache/pulsar/pull/10822 ([@fantapsody](https://github.com/fantapsody))


### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - 023: June Project Updates on Apache Pulsar

      - https://www.youtube.com/watch?v=MTHE3_cUekc

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Pulsar User Survey 2021 Highlights

    - https://streamnative.io/en/blog/community/2021-06-11-pulsar-user-survey-2021-highlights

- 2021 Apache Pulsar User Report Announcement

    - https://streamnative.io/en/blog/community/2021-06-10-2021-apache-pulsar-user-report-announcement

- Keynotes Announced for Pulsar Virtual Summit North America 2021

    - https://streamnative.io/en/blog/community/2021-06-09-keynotes-announced-for-pulsar-virtual-summit-north-america-2021

- What’s New in Apache Pulsar 2.6.4

    - https://streamnative.io/en/blog/release/2021-06-08-pulsar-264

- Matteo Merli, Apache Pulsar PMC Chair, Joins StreamNative as CTO

    - https://streamnative.io/en/blog/community/2021-06-08-matteo-merli-apache-pulsar-pmc-chair-joins-streamnative-as-cto

- Four Reasons Why Apache Pulsar is Essential to the Modern Data Stack

    - https://datastax.medium.com/four-reasons-why-apache-pulsar-is-essential-to-the-modern-data-stack-b90a8bddcb9

- Apache Pulsar Demonstrates Best-in-Class Cloud-Native Price-Performance

    - https://gigaom.com/2021/06/11/apache-pulsar-demonstrates-best-in-class-cloud-native-price-performance/