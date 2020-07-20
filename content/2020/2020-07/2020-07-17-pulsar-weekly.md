---
title: "2020-07-17-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-07-11 ~ 2020-07-17"
date: 2020-07-11 ~ 2020-07-17
description: "This is the Pulsar community weekly update for 2020-07-11 ~ 2020-07-17, with updates on Pulsar clients, broker, Functions, and so on."
id: "2020-07-17-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-07-11 ~ 2020-07-17

This is the Pulsar community weekly update for 2020-07-11 ~ 2020-07-17, with updates on Pulsar authentication, broker, Functions, and so on.

### Notable Feature

- [Pulsar Functions] Improve security setting of Pulsar Functions.

    https://github.com/apache/pulsar/pull/7578

- [Pulsar Functions] Support different docker images in Kubernetes runtime of Pulsar Functions.
  
    https://github.com/apache/pulsar/pull/6752

- [Pulsar Client] Support setting customized retry delay for consumers.
  
    https://github.com/apache/pulsar/pull/6449

- [Build] Add limited module set profile to the POM files.
  
    https://github.com/apache/pulsar/pull/7541

- [Build] Update Jersey version to v2.31.

    https://github.com/apache/pulsar/pull/7515

- [Build] Update Jackson version to v2.11.1 and ensure all dependencies are pinned.
  
    https://github.com/apache/pulsar/pull/7519

- [Build] Use GitHub actions cache for Maven dependencies.
  
    https://github.com/apache/pulsar/pull/7527

### Notable Bug Fix

- [Broker] Introduce a timeout mechanism in the managed ledger factory.

    https://github.com/apache/pulsar/pull/7506

- [Pulsar Client] Handle NotAllowed Exception at the client side.

    https://github.com/apache/pulsar/pull/7430

- [PROTOBUF] Fix protobuf generation on handling repeated long number.

    https://github.com/apache/pulsar/pull/7540

- [Pulsar Client] Ensure the create subscription can be completed when the operation timeout happens.

    https://github.com/apache/pulsar/pull/7522

- [Pulsar Client] Decompress payload if needed in KeyShared subscription.

    https://github.com/apache/pulsar/pull/7416

- [Pulsar Functions] Fix function BC issue introduced in release 2.6.0.

    https://github.com/apache/pulsar/pull/7528

- [Broker] Clean deleted topics from the namespace.

    https://github.com/apache/pulsar/pull/7473

- [Broker] Fix the issue that topic is recreated immediately after deletion.

    https://github.com/apache/pulsar/pull/7524

- [Pulsar Functions] When a function worker becomes the leader, start producer to assignment topic first before stopping the assignment tailer.

    https://github.com/apache/pulsar/pull/7525

### Event / News

- [Pulsar Summit] The first-ever Pulsar Summit Virtual Conference 2020 was held on June 17 - 18. This two-day digital event featured more than 30 sessions from top Pulsar contributors and developers.

    All video recordings and slides are available at [here](https://streamnative.io/resource#pulsar-summit). 
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    All video recordings are available at [here](https://streamnative.io/resource#tgip).

- Upcoming events

  - 07/28: StreamNative Webinar - "How to Operate Pulsar in Production" by Matteo Merli, Joe Frances, Sijie Guo, and Addison Higham

        Registration link: https://us02web.zoom.us/webinar/register/WN_xMt6QBJ9TWiyeVdifqKITg

### Blog / Article

- Taking messaging and data ingestion systems to the next level - Sijie Guo

    https://streamnative.io/blog/tech/2020-07-08-podcast
