---
title: "2020-07-31-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-07-25 ~ 2020-07-31"
date: 2020-07-25 ~ 2020-07-31
description: "This is the Pulsar community weekly update for 2020-07-25 ~ 2020-07-31, with updates on Pulsar clients, Functions, broker, transaction, security, and so on."
id: "2020-07-31-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-07-25 ~ 2020-07-31

This is the Pulsar community weekly update for 2020-07-25 ~ 2020-07-31, with updates on Pulsar clients, Functions, broker, transaction, security, and so on.

### Notable Feature

- [Broker] Support setting backlog quota on topic level.

    https://github.com/apache/pulsar/pull/7646

- [Pulsar client] Remove UUID generation on sending message.

    https://github.com/apache/pulsar/pull/7705

- [Pulsar client] Close the hanging thread after Pulsar Admin Java Client is closed.

    https://github.com/apache/pulsar/pull/7687

- [Pulsar client] Fix backward compatibility issues with batch index acknowledgment.

    https://github.com/apache/pulsar/pull/7655

- [Pulsar client] Support configuring `DeleteInactiveTopic` in namespace policy.

    https://github.com/apache/pulsar/pull/7598

- [Functions] Add additional metrics for the Pulsar Function Worker.

    https://github.com/apache/pulsar/pull/7685

- [Transaction] Implement the Transaction Buffer Client.

    https://github.com/apache/pulsar/pull/6544

- [Security] Use Consume/Produce/Lookup interfaces for specific operations in `allowTopicOperation`.

    https://github.com/apache/pulsar/pull/7587

### Notable Bug Fix

- [Pulsar client] Fix race condition on the closed consumer while reconnecting to the broker.

    https://github.com/apache/pulsar/pull/7589

- [Pulsar client] Fix segment crashes that are caused by race condition of the timer in the C++ client.

    https://github.com/apache/pulsar/pull/7572

- [Pulsar client] Fix the issue that the `batchReceiveAsync` is not completed exceptionally when the consumer is closed.

    https://github.com/apache/pulsar/pull/7661

- [Pulsar client] Fix batch index filtering issue in the consumer.

    https://github.com/apache/pulsar/pull/7654

- [Pulsar client] Fix the time unit error of the producer stats recorder.

    https://github.com/apache/pulsar/pull/7670

- [Broker] Fix race condition on deleted topic with active readers.

    https://github.com/apache/pulsar/pull/7715

- [Broker] Introduce a timeout of opening managed ledger.

    https://github.com/apache/pulsar/pull/7506

- [Broker] Fix the issue that deduplication cursor is not deleted after the message deduplication is disabled.

    https://github.com/apache/pulsar/pull/7656

- [Broker] Fix NPE when using `advertisedListeners`.

    https://github.com/apache/pulsar/pull/7620

### Event / News

- [Pulsar Summit] The first-ever Pulsar Summit Virtual Conference 2020 was held on June 17 - 18. This two-day digital event featured more than 30 sessions from top Pulsar contributors and developers.

    All video recordings and slides are available at [here](https://streamnative.io/resource#pulsar-summit).
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 017: Pulsar Multi-Tenancy Best Practices
  
        - https://www.youtube.com/watch?v=2zGBJNLhO44

- [Webinar]

  - 07/28: StreamNative Webinar - "How to Operate Pulsar in Production" by Matteo Merli, Joe Frances, Addison Higham, and Sijie Guo

    Recording: https://www.youtube.com/watch?v=mncXc_T6JkU

### Blog / Article

- Pulsar vs. Kafka: A More Accurate Perspective from Use Cases and Community to Features and Performance

    - https://streamnative.io/whitepaper/pulsar-vs-kafka
