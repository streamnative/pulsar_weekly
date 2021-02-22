---
title: "2021-02-15-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-02-08 ~ 2021-02-14"
date: 2021-02-08 ~ 2021-02-14
description: "This is the Pulsar community weekly update for 2021-02-08 ~ 2021-02-14, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-02-15-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-02-08 ~ 2021-02-14

This is the Pulsar community weekly update for 2021-02-08 ~ 2021-02-14, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Pulsar Highlight

Pulsar does not need to run as the root user. Therefore, Pulsar and the Pulsar dashboard images are updated to run as a new Pulsar user (User 1000 10000 and Group 10001). This change increases the security of Pulsar images.

by ([michaeljmarshall](https://github.com/michaeljmarshall))

### Notable Feature

- [Broker] Authorization service uses the metadata-store API.

    https://github.com/apache/pulsar/pull/9586 (@[rdhabalia](https://github.com/rdhabalia))

- [Flaky Test] Pass "alwaysRun = true" to all TestNG @After* annotations Consistently.

    https://github.com/apache/pulsar/pull/9635 (@[lhotari](https://github.com/lhotari))

- [Build] Add `-parameters` flag in javac.

    https://github.com/apache/pulsar/pull/9624 (@[Renkai](https://github.com/Renkai))

- [Transaction] Enable SpotBugs in the pulsar-transaction module.

    https://github.com/apache/pulsar/pull/9620 (@[congbobo184](https://github.com/congbobo184))

- [Broker] Support enabling subscription types.

    https://github.com/apache/pulsar/pull/9401 (@[congbobo184](https://github.com/congbobo184))

- [Python] Support end-to-end encryption.

    https://github.com/apache/pulsar/pull/9588 (@[tuteng](https://github.com/tuteng))

- [CLI] pulsar-client CLI tool supports end-to-end encryption.

    https://github.com/apache/pulsar/pull/9615 (@[massakam](https://github.com/massakam))

- [Broker] Topic resources use the metadata-store API.

    https://github.com/apache/pulsar/pull/9485 (@[rdhabalia](https://github.com/rdhabalia))

- [Pulsar Admin] Expose schema ledger in `topic stats-internal`.

    https://github.com/apache/pulsar/pull/9284 (@[congbobo184](https://github.com/congbobo184))

- [Function] Enable Function Workers to use the exclusive producer to write messages to internal topics.

    https://github.com/apache/pulsar/pull/9275 (@[jerrypeng](https://github.com/jerrypeng))

- [Metrics] Add producer metrics for Prometheus.

    https://github.com/apache/pulsar/pull/9541 (@[wangjialing218](https://github.com/wangjialing218))

- [Function] The Kubernetes runtime functions creates REC1123-compliant labels.

    https://github.com/apache/pulsar/pull/9556 (@[jdbeck](https://github.com/jdbeck))

- [Build] Update the Docker file for Pulsar and Dashboard to create and use the Pulsar user (non-root user).

    https://github.com/apache/pulsar/pull/8796 (@[michaeljmarshall](https://github.com/michaeljmarshall))

- [Function] Set the maximum allowed amount of resources for Pulsar Functions.

    https://github.com/apache/pulsar/pull/9584 (@[fantapsody](https://github.com/fantapsody))

- [C++] Make pool connections configurable in pulsar-perf CLI tool.

    https://github.com/apache/pulsar/pull/8913 (@[ltamber](https://github.com/ltamber))

- [Pulsar-IO] Add option for `auto.offset.reset` to the Kafka Source connector.

    https://github.com/apache/pulsar/pull/9482 (@[sbourkeostk](https://github.com/sbourkeostk))

- [CLI] Add user-friendly comments for the topic compactor tool.

    https://github.com/apache/pulsar/pull/9563 (@[WJL3333](https://github.com/WJL3333))

### Notable Bug Fix

- [Client] Fix `hasMessageAvailable()` with the empty topic.

    https://github.com/apache/pulsar/pull/9652 (@[jerrypeng](https://github.com/jerrypeng))

- [Build] Remove `pom.xml` file from pulsar-functions-worker-shaded which is no longer used.

    https://github.com/apache/pulsar/pull/9637 (@[lhotari](https://github.com/lhotari))

- [Broker] Remove `global-zk` reference from Pulsar-service.

    https://github.com/apache/pulsar/pull/9648 (@[rdhabalia](https://github.com/rdhabalia))

- [Client] Fix writing/encoding of `GenericJsonRecord`.

    https://github.com/apache/pulsar/pull/9608 (@[lhotari](https://github.com/lhotari))

- [Bookie] Fallback to `PULSAR_GC` if `BOOKIE_GC` is not defined.

    https://github.com/apache/pulsar/pull/9621 (@[lhotari](https://github.com/lhotari))

- [Build] Reduce the `pulsar-test-latest-version` docker image size.

    https://github.com/apache/pulsar/pull/9627 (@[lhotari](https://github.com/lhotari))

- [Flaky Test] Fix the Bookie's `dbStorage_*CacheMaxSizeMb` setting in `pulsar-test-latest-version` docker image.

    https://github.com/apache/pulsar/pull/9623 (@[lhotari](https://github.com/lhotari))

- [Broker] Fix the timeout operation when the `wait-for-exclusive` producer is handled incorrectly.

    https://github.com/apache/pulsar/pull/9600 (@[merlimat](https://github.com/merlimat))

- [Client] Add `BouncyCastleProvider` as the security provider to prevent NPE.

    https://github.com/apache/pulsar/pull/9601 (@[massakam](https://github.com/massakam))

- [Build] Fix expired TLS certificates for C++ tests.

    https://github.com/apache/pulsar/pull/9607 (@[sijie](https://github.com/sijie))

- [Broker] Fix NPE that occurs in `PersistentStickyKeyDispatcherMultipleConsumers` when debug log is enabled.

    https://github.com/apache/pulsar/pull/9587 (@[massakam](https://github.com/massakam))

- [Broker] Only log `auth _errors_ ` at the error level.

    https://github.com/apache/pulsar/pull/9325 (@[ivankelly](https://github.com/ivankelly))

- [Admin] Fix the NPE that occurs when getting messages by the ID while the message is null.

    https://github.com/apache/pulsar/pull/9537 (@[315157973](https://github.com/315157973))

- [Admin CLI] Inform users when the request for expiring messages is not executed.

    https://github.com/apache/pulsar/pull/9561 (@[MarvinCai](https://github.com/MarvinCai))

- [Build] Disable looking up snapshot versions in public repositories.

    https://github.com/apache/pulsar/pull/9336 (@[lhotari](https://github.com/lhotari))

- [Python] Match BookKeeper's `grpcio` requirement.

    https://github.com/apache/pulsar/pull/9569 (@[jbellis](https://github.com/jbellis))

- [Broker] Fix the race condition in `BrokerService` topic cache.

    https://github.com/apache/pulsar/pull/9565 (@[lhotari](https://github.com/lhotari))

- [Client] Clean up consumers on multi-topic subscribe failure.

    https://github.com/apache/pulsar/pull/9419 (@[addisonj](https://github.com/addisonj))

- [FlakyTest] Fix NPEs in test cleanup methods.

    https://github.com/apache/pulsar/pull/9442 (@[Wzhipeng](https://github.com/Wzhipeng))

- [FlakyTest] Fix failed `LoadReportNetworkLimit` test.

    https://github.com/apache/pulsar/pull/9581 (@[lhotari](https://github.com/lhotari))

- [Build] Avoid introducing BookKeeper-common into the pulsar-common.

    https://github.com/apache/pulsar/pull/9551 (@[zymap](https://github.com/zymap))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 019: Latest Updates On Apache Pulsar
  
        - https://www.youtube.com/watch?v=EkRULmkaWGY

### Blog / Article

- StreamNative's 2020 Year in Review

    - https://streamnative.io/en/blog/community/2021-02-16-streamnative-2020-year-in-review
