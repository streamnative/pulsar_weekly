---
title: "2020-11-27-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-11-21 ~ 2020-11-27"
date: 2020-11-21 ~ 2020-11-27
description: "This is the Pulsar community weekly update for 2020-11-21 ~ 2020-11-27, with updates on Pulsar client, broker, transactions, Functions, schema, tiered storage, and so on."
id: "2020-11-27-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-11-21 ~ 2020-11-27

This is the Pulsar community weekly update for 2020-11-21 ~ 2020-11-27, with updates on Pulsar client, broker, transactions, Functions, schema, tiered storage, and so on.

### Pulsar Highlight

- Add the transactions log for Pulsar and implementation of PIP-31.

    https://github.com/apache/pulsar/wiki/PIP-31%3A-Transaction-Support

    by (@[congbobo184](https://github.com/congbobo184))

- Introduce the package management interface API and implementation of PIP-50.

    https://github.com/apache/pulsar/wiki/PIP-50%3A-Package-Management

    by (@[zymap](https://github.com/zymap))

- Support the HAProxy proxy protocol for the Pulsar broker and Pulsar proxy.

    https://github.com/apache/pulsar/pull/8686

    by (@[codelipenghui](https://github.com/codelipenghui))

### Notable Feature

- [Transactions] Add the transactions log for Pulsar.

    https://github.com/apache/pulsar/pull/8658 (@[congbobo184](https://github.com/congbobo184))

- [Pulsar Functions] Add E2E documents for Pulsar Functions.

    https://github.com/apache/pulsar/pull/8648 (@[wolfstudy](https://github.com/wolfstudy))

- [Java Client] Expose the receiver queue size to the client consumer stats.

    https://github.com/apache/pulsar/pull/8663 (@[315157973](https://github.com/315157973))

- [Broker] Introduce the package management interface API.

    https://github.com/apache/pulsar/pull/8669 (@[congbobo184](https://github.com/congbobo184))

- [Broker] Support the HAProxy proxy protocol for the Pulsar broker and Pulsar proxy.

    https://github.com/apache/pulsar/pull/8686 (@[codelipenghui](https://github.com/codelipenghui))

- [Pulsar Functions] Add timeout to `hasMessageAvailable` to the leader election process in Pulsar Functions.

    https://github.com/apache/pulsar/pull/8687 (@[jerrypeng](https://github.com/jerrypeng))

### Notable Bug Fix

- [Broker] Use `Awaitility` instead `Thread.sleep` in `InactiveTopicDeleteTest.java`.

    https://github.com/apache/pulsar/pull/8647 (@[315157973](https://github.com/315157973))

- [Broker] Fix the Apache rat check issue.

    https://github.com/apache/pulsar/pull/8665 (@[codelipenghui](https://github.com/codelipenghui))

- [Broker] Clear delayed messages when clearing the backlog.

    https://github.com/apache/pulsar/pull/8691 (@[codelipenghui](https://github.com/codelipenghui))

- [Tiered Storage] Fix the Jclouds Azure credential error.

    https://github.com/apache/pulsar/pull/8693 ([@gaoran10](https://github.com/gaoran10))

- [Build] Update the management module version.

    https://github.com/apache/pulsar/pull/8695 ([@gaoran10](https://github.com/gaoran10))

- [Build] Upgrade the license-maven-plugin to version 4.0.rc2.

    https://github.com/apache/pulsar/pull/8706 ([@lhotari](https://github.com/lhotari))

- [Build] Fix the issue in Maven build that re-compiles all classes.

    https://github.com/apache/pulsar/pull/8707 ([@lhotari](https://github.com/lhotari))

- [Build] Specify the `maven-antrun-plugin` version and migrate it to use the newer syntax.

    https://github.com/apache/pulsar/pull/8708 ([@lhotari](https://github.com/lhotari))

- [CI] Fix the the issue that the "CI - Build - Multiple - OS" fails on the `macos-latest` runner.

    https://github.com/apache/pulsar/pull/8713 ([@lhotari](https://github.com/lhotari))

- [Java Client] Include `com.google.guava:failureaccess` in the shaded JAR.

    https://github.com/apache/pulsar/pull/8697 ([@cimura](https://github.com/cimura))

- [Prometheus Metrics] Update the PrometheusMetrics on binaries when building from the source tarball.

    https://github.com/apache/pulsar/pull/8702 (@[eolivelli](https://github.com/eolivelli))

- [Log Conf] Delete the explicit claim for the log configuration file position in surefire.

    https://github.com/apache/pulsar/pull/8715 ([@Renkai](https://github.com/Renkai))

- [WebSocket] Fix the initial sequence ID error.

    https://github.com/apache/pulsar/pull/8724 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Java Client] Fix the warning log on the producer side when duplicated message is dropped.

    https://github.com/apache/pulsar/pull/8729 ([@massakam](https://github.com/massakam))

- [Unit Test] Fix the `MessagePublishBufferThrottleTest` flaky-test.

    https://github.com/apache/pulsar/pull/8733 (@[315157973](https://github.com/315157973))

- [Unit Test] Fix the `TopicsConsumerImplTest.testConsumerUnackedRedelivery` flaky-test.

    https://github.com/apache/pulsar/pull/8738 (@[315157973](https://github.com/315157973))

- [Tiered Storage] Initialize the offload manager only for one time.

    https://github.com/apache/pulsar/pull/8739 ([@gaoran10](https://github.com/gaoran10))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020å

### Blog / Article

- Apache Pulsar-as-a-Service Launches on Alibaba Cloud

  - https://streamnative.io/en/blog/release/2020-11-25-streamnative-alibaba-cloud

- Powering Federated Learning at Tencent with Apache Pulsar

  - https://streamnative.io/en/blog/case/2020-11-26-tencent-angle

- Comparing Pulsar and Kafka From a CTO’s Point of View -- Jesse Anderson 

  - https://dzone.com/articles/comparing-pulsar-and-kafka-from-a-ctos-point-of-vi

- The choice of Apache Pulsar -- Gilles Barbier

  - https://infinitic.substack.com/p/the-choice-of-apache-pulsar
