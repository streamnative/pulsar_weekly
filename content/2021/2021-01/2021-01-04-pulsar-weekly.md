---
title: "2021-01-04-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-12-28 ~ 2021-01-03"
date: 2020-12-28 ~ 2021-01-03
description: "This is the Pulsar community weekly update for 2020-12-28 ~ 2021-01-03, with updates on Pulsar client, broker, Functions, and so on."
id: "2021-01-04-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-12-28 ~ 2021-01-03

This is the Pulsar community weekly update for 2020-12-28 ~ 2021-01-03, with updates on Pulsar client, broker, Functions, and so on.

### Pulsar Highlight

Expose the end-to-end encryption interface for the C++ client to make users use the end-to-end encryption on other clients, such as the Python client or the Node.js clients.

by [tuteng](https://github.com/tuteng)

### Notable Feature

- [Pulsar Functions] Support the package command in Pulsar Functions.

    https://github.com/apache/pulsar/pull/8973 ([zymap](https://github.com/zymap))

- [Pulsar Functions] Support creating and updating the source with the package name.

    https://github.com/apache/pulsar/pull/8988  ([zymap](https://github.com/zymap))

- [C++] Expose the end-to-end encryption interface.

    https://github.com/apache/pulsar/pull/9074 ([tuteng](https://github.com/tuteng))

### Notable Bug Fix

- [Pulsar IO] Fix the error log of the Debezium connector.

    https://github.com/apache/pulsar/pull/9063 ([yufan022](https://github.com/yufan022))

- [Placement Policy] Fix the issue that the AutoRecovery does not respect to the isolation group settings.

    https://github.com/apache/pulsar/pull/8961  ([zymap](https://github.com/zymap))

- [C++] Fix the issue that the C++ client does not clean up previous messages when implementing the `AcknowledgeCumulative` operation.

    https://github.com/apache/pulsar/pull/8606 ([saosir](https://github.com/saosir))

- [Broker] Fix the issue that occurs when the master broker wants to subscribe to a partitioned non-persistent topic with the topic auto-creation being disabled.

    https://github.com/apache/pulsar/pull/9107 ([codelipenghui](https://github.com/codelipenghui))

- Fix the regression in `apply-config-from-env.py`.

    https://github.com/apache/pulsar/pull/9097 ([codelipenghui](https://github.com/codelipenghui))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq

### Blog / Article

- Apache Pulsar vs. Kafka and other data processing technologies -- David Kjerrumgaard

    - https://searchdatamanagement.techtarget.com/post/Apache-Pulsar-vs-Kafka-and-other-data-processing-technologies

- How to implement asynchronous replication in Apache Pulsar -- David Kjerrumgaard

    - https://searchdatabackup.techtarget.com/post/How-to-implement-asynchronous-replication-in-Apache-Pulsar
