---
title: "2020-07-24-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-07-18 ~ 2020-07-24"
date: 2020-07-18 ~ 2020-07-24
description: "This is the Pulsar community weekly update for 2020-07-18 ~ 2020-07-24, with updates on Pulsar clients, Functions, and so on."
id: "2020-07-24-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-07-18 ~ 2020-07-24

This is the Pulsar community weekly update for 2020-07-18 ~ 2020-07-24, with updates on Pulsar authentication, broker, Functions, and so on.

### Notable Feature

- [Functions] Reduce the leader initiation time in Pulsar Functions.

    https://github.com/apache/pulsar/pull/7611

- [Functions] Add readiness API for the Function worker leader.

    https://github.com/apache/pulsar/pull/7601

- [Functions] Export Function worker internal stats via Prometheus.

    https://github.com/apache/pulsar/pull/7641

- [Functions] Allow ability to specify retain key ordering in Pulsar Functions.

    https://github.com/apache/pulsar/pull/7647

### Notable Bug Fix

- [CPP Client] Fix multitopic consumer segfault on connection error.

    https://github.com/apache/pulsar/pull/7588

- [Functions] Fix the issue that the dead letter topic is not the same as enableRetry in Pulsar Functions.

    https://github.com/apache/pulsar/pull/7610

### Event / News

- [Pulsar Summit] The first-ever Pulsar Summit Virtual Conference 2020 was held on June 17 - 18. This two-day digital event featured more than 30 sessions from top Pulsar contributors and developers.

    All video recordings and slides are available at [here](https://streamnative.io/resource#pulsar-summit).
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 016: Backlog and StorageSize - Understand why the storage of your Pulsar cluster is filling up - Sijie Guo
  
        - https://www.youtube.com/watch?v=PIX570nyq_c

- Upcoming events

  - 07/28: StreamNative Webinar - "How to Operate Pulsar in Production" by Matteo Merli, Joe Frances, Addison Higham and Sijie Guo

    Registration link: https://us02web.zoom.us/webinar/register/WN_xMt6QBJ9TWiyeVdifqKITg

### Blog / Article

- Pulsar vs. Kafka: A More Accurate Perspective from Features and Performance to Use Cases and Community

    - https://streamnative.io/whitepaper/pulsar-vs-kafka

- Pulsar vs Kafka - Part 2 - Adoption, Use Cases, Differentiators, and Community

    - https://streamnative.io/blog/tech/pulsar-vs-kafka-part-2

- Event-driven Functions with Apache Pulsar & Project Flogo - Matt Ellis

    - https://hackernoon.com/event-driven-functions-with-apache-pulsar-and-project-flogo-wag3y4u