---
title: "2021-03-08-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-03-01 ~ 2021-03-07"
date: 2021-03-01 ~ 2021-03-07
description: "This is the Pulsar community weekly update for 2021-03-01 ~ 2021-03-07, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-03-08-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-03-01 ~ 2021-03-07

This is the Pulsar community weekly update for 2021-03-01 ~ 2021-03-07, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Pulsar Highlight

- [broker] Allow to enable or disable the cursor metrics.

  https://github.com/apache/pulsar/pull/9814 ([@linlinnn](https://github.com/linlinnn))
  
- [Transactions] Handle TC low water mark on pending ack handle.

  https://github.com/apache/pulsar/pull/9722 ([@congbobo184](https://github.com/congbobo184))

### Notable Feature

- [Common] Ensure read-lock is not continuously held on a section while iterating over concurrent maps.

  https://github.com/apache/pulsar/pull/9787 ([@merlimat](https://github.com/merlimat))

- [Utils] Dump JVM information for pulsar-perf.

  https://github.com/apache/pulsar/pull/9769 ([@eolivelli](https://github.com/eolivelli))

- [Broker] Support getting applied `BlacklogQuota`.

  https://github.com/apache/pulsar/pull/9828 ([@315157973](https://github.com/315157973))

- [Broker] Support getting applied `SubscriptionDispatchRate`.

  https://github.com/apache/pulsar/pull/9827 ([@315157973](https://github.com/315157973))
  
- [CI] Before retrying or proceeding to next methods, clean up the test state after a failure.

  https://github.com/apache/pulsar/pull/9823 ([@lhotari](https://github.com/lhotari))

- [C++ client] Remove the `gtest` file from the C++ library.

  https://github.com/apache/pulsar/pull/9816 ([@zymap](https://github.com/zymap))

- [CI] Add apache-rat check in CI test.

  https://github.com/apache/pulsar/pull/9815 ([@zymap](https://github.com/zymap))
  
- [Build] Remove the DEB package from the Pulsar docker image.

  https://github.com/apache/pulsar/pull/9811 ([@merlimat](https://github.com/merlimat))

- [Build] Split `pulsar-io-kafka-connect-adaptor` into JAR and NAR modules.

  https://github.com/apache/pulsar/pull/9808 ([@merlimat](https://github.com/merlimat))
  
- [Broker] Add pending read subscription metrics to stats-internal.

  https://github.com/apache/pulsar/pull/9788 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Add NPE check for `PulsarService#getAdminClient`.

  https://github.com/apache/pulsar/pull/9782 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Build] Enable detailed Java compiler warnings.

  https://github.com/apache/pulsar/pull/9780 ([@lhotari](https://github.com/lhotari))

- [Build] Update the Pulsar version in the terraform file when setting the project version.

  https://github.com/apache/pulsar/pull/9775 ([@zymap](https://github.com/zymap))

- [Deployment] Update the Pulsar version to 2.7.0 for the ansible deployment.

  https://github.com/apache/pulsar/pull/9774 ([@codelipenghui](https://github.com/codelipenghui))

- [CI] Refactor integration test commands to the `run_integration_group.sh` script.

  https://github.com/apache/pulsar/pull/9770 ([@lhotari](https://github.com/lhotari))

- [CI] Use `DiagnosticCommand` JMX MBean to do the thread dump.

  https://github.com/apache/pulsar/pull/9766 ([@lhotari](https://github.com/lhotari))

- [CI] Reduce the size of integration test image by only including selected connectors.

  https://github.com/apache/pulsar/pull/9807 ([@merlimat](https://github.com/merlimat))
  
- [Go client] Update JWT-Go version to v4.

  https://github.com/apache/pulsar-client-go/pull/481 ([@fanjeff](https://github.com/fanjeff))
  
- [Broker] Prevent using invalid broker or proxy configurations for authorization.

  https://github.com/apache/pulsar/pull/9746 ([@lhotari](https://github.com/lhotari))
  
- [Broker] Change the `getWorkerService` method to throw `UnsupportedOperationException`.

  https://github.com/apache/pulsar/pull/9738 ([@golden-yang](https://github.com/golden-yang))
  
- [Broker] Do not add the broker-address header if the response has already been committed.

  https://github.com/apache/pulsar/pull/9744 ([@lhotari](https://github.com/lhotari))
  
- [Broker] Validate the offload parameter.

  https://github.com/apache/pulsar/pull/9737 ([@patricklucas](https://github.com/patricklucas))
  
- [transaction] Retry TC-end transactions.

  https://github.com/apache/pulsar/pull/9236 ([@congbobo184](https://github.com/congbobo184))

### Notable Bug Fix
  
- [Broker] Fix `hasMessageAvailable()` with the empty topic (branch 2.7).

  https://github.com/apache/pulsar/pull/9798 ([@zymap](https://github.com/zymap))

- [Broker] Fix the issue that the topic ownership is not checked when getting topic-applied policies (branch 2.7).

  https://github.com/apache/pulsar/pull/9781 ([@315157973](https://github.com/315157973))

- [Broker] Fix the issue that the topic ownership is not checked when get topic-applied policies (master branch).

  https://github.com/apache/pulsar/pull/9767 ([@315157973](https://github.com/315157973))
  
- [Broker] Fix NPEs and the thread safety issue in `PersistentReplicator`.

  https://github.com/apache/pulsar/pull/9763 ([@lhotari](https://github.com/lhotari))

- [Java client] Fix the NPE in `ClientCnx`.

  https://github.com/apache/pulsar/pull/9761 ([@lhotari](https://github.com/lhotari))

- [Broker] Fix the issue that the consumer fails to use the older subscriptions to consume messages if the maximum subscription limit is reached.

  https://github.com/apache/pulsar/pull/9758 ([@315157973](https://github.com/315157973))

- [Go client] Fix the socket leakage in the lookup service.

  https://github.com/apache/pulsar-client-go/pull/478 ([@freeznet](https://github.com/freeznet))
  
- [Transactions] Fix the append sync problem of the transaction log.

  https://github.com/apache/pulsar/pull/9238 ([@congbobo184](https://github.com/congbobo184))

### Event / News

- [Webinar] TiDB + Pulsar, Event Streaming Architecture in Action

  - https://www.youtube.com/watch?v=_IPWv1shCDc

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Taking an In-Depth Look at How to Achieve Isolation in Pulsar

    - https://streamnative.io/en/blog/tech/2021-03-02-taking-an-in-depth-look-at-how-to-achieve-isolation-in-pulsar

- Ververica + StreamNative: Cloud Partners

    - https://streamnative.io/en/blog/community/2021-03-03-ververica-streamantive-cloud-partners
