---
title: "2021-02-22-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-02-15 ~ 2021-02-21"
date: 2021-02-15 ~ 2021-02-21
description: "This is the Pulsar community weekly update for 2021-02-15 ~ 2021-02-21, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-02-22-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-02-15 ~ 2021-02-21

This is the Pulsar community weekly update for 2021-02-15 ~ 2021-02-21, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Pulsar Highlight

Support handling messages with multiple listener threads for the Key_Shared subscription. Currently, a consumer is pinged to a given listener thread to ensure that the message is processed orderly for a topic. But for the Key_Shared subscription, the message process order is based on the message key, not the order of the topic. Therefore, we create a feature to support handling messages with multiple listener threads for the Key_Shared subscription to ensure the order of the message key.

by (@[codelipenghui](https://github.com/codelipenghui))

### Notable Feature

- [Client] Support handling messages with multiple listener threads for the Key_Shared subscription.

    https://github.com/apache/pulsar/pull/9329 (@[codelipenghui](https://github.com/codelipenghui))

- [Build] Build Pulsar with unix lineEnding in Windows.

    https://github.com/apache/pulsar/pull/9536 (@[wangjialing218](https://github.com/wangjialing218))

- [Build] Support building Pulsar with JDK11 and `-Dmaven.compiler.release=8`.

    https://github.com/apache/pulsar/pull/9580 (@[eolivelli](https://github.com/eolivelli))

- [C++] Support disabling static or dynamic libraries at the build time.

    https://github.com/apache/pulsar/pull/9570 (@[merlimat](https://github.com/merlimat))

- [C++] Account for different variables names on different CMake versions.

    https://github.com/apache/pulsar/pull/9559 (@[merlimat](https://github.com/merlimat))

- [C++] Add detail logs for schema related messages.

    https://github.com/apache/pulsar/pull/9544 (@[BewareMyPower](https://github.com/BewareMyPower))

- [CLI] Add the command used for listing bookies for pulsar-admin CLI tool.

    https://github.com/apache/pulsar/pull/9283 (@[eolivelli](https://github.com/eolivelli))

- [C++] Remove usages of `boost::regex`.

    https://github.com/apache/pulsar/pull/9533 (@[merlimat](https://github.com/merlimat))

- [CLI] Expire messages by the position.

    https://github.com/apache/pulsar/pull/9514 (@[MarvinCai](https://github.com/MarvinCai))

- [Broker] Asynchronously read entries with the maximum size bytes.

    https://github.com/apache/pulsar/pull/9532 (@[gaoran10](https://github.com/gaoran10))

- [Broker] Disallow parsing token without signature in `authenticateToken`.

    https://github.com/apache/pulsar/pull/9172 (@[nodece](https://github.com/nodece))

- [Function] Add `downloadDirectory` support to Kubernetes runtime.

    https://github.com/apache/pulsar/pull/9377 (@[freeznet](https://github.com/freeznet))

- [Broker] ENsure that the subscription starts from `MessageId.latest` by default.

    https://github.com/apache/pulsar/pull/9444 (@[aloyszhang](https://github.com/aloyszhang))

- [CI] Replace the `diff-only` action with the usage of `paths-ignore`.

    https://github.com/apache/pulsar/pull/9527 (@[lhotari](https://github.com/lhotari))

- [Function/IO] Optimize built-in source/sink startup.

    https://github.com/apache/pulsar/pull/9500 (@[jerrypeng](https://github.com/jerrypeng))

- [Broker] Ignore `.replicateSubscriptionState(true)` setting When replicated subscription is disabled by Pulsar broker.

    https://github.com/apache/pulsar/pull/9523 (@[k2la](https://github.com/k2la))

- [Broker] Namespace resources use the metadata-store API.

    https://github.com/apache/pulsar/pull/9351 (@[rdhabalia](https://github.com/rdhabalia))

- [TestClient] Add `--batch-index-ack` for the pulsar-perf CLI tool.

    https://github.com/apache/pulsar/pull/9521 (@[limingnihao](https://github.com/limingnihao))

- [Broker] Add subscription backlog size information for `topicstats`.

    https://github.com/apache/pulsar/pull/9302 (@[MarvinCai](https://github.com/MarvinCai))

- [Pulsar Common] Add user-friendly error hint to tell users the expected namespace format when getting errors in the namespace parse.

    https://github.com/apache/pulsar/pull/9510 (@[Renkai](https://github.com/Renkai))

### Notable Bug Fix

- [Functions] Close `InputStreams` properly.

    https://github.com/apache/pulsar/pull/9568 (@[lhotari](https://github.com/lhotari))

- [Flaky Test] Fix the flaky test `BrokerServiceLookupTest.testModularLoadManagerSplitBundle`.

    https://github.com/apache/pulsar/pull/9577 (@[lhotari](https://github.com/lhotari))

- [Docker] Fix incorrect URL in README for docker-compose.

    https://github.com/apache/pulsar/pull/9573 (@[aahmed-se](https://github.com/aahmed-se))

- [Build] Add missing Python 3.9 paths in `CmakeLists.txt`.

    https://github.com/apache/pulsar/pull/9574 (@[aahmed-se](https://github.com/aahmed-se))

- [Python] Initialize Python 3.9 client wheel build.

    https://github.com/apache/pulsar/pull/9389 (@[vkvm](https://github.com/vkvm))

- [Python] Fix nested `Map` or `Array` in schema that doesn't work.

    https://github.com/apache/pulsar/pull/9548 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Client] Fix a couple of bugs in the exclusive producer.

    https://github.com/apache/pulsar/pull/9554 (@[jerrypeng](https://github.com/jerrypeng))

- [C++] Add the `encrypted` option in `commands.newproducer()`.

    https://github.com/apache/pulsar/pull/9542 (@[wineway](https://github.com/wineway))

- [Client] Make the DLQ process asynchronous.

    https://github.com/apache/pulsar/pull/9552 (@[codelipenghui](https://github.com/codelipenghui))

- [FlakyTest] Fix `testBrokerSelectionForAntiAffinityGroup` by increasing `OverloadedThreshold`.

    https://github.com/apache/pulsar/pull/9393 (@[michaeljmarshall](https://github.com/michaeljmarshall))

- [Functions] Call the corresponding restart according to the component type.

    https://github.com/apache/pulsar/pull/9519 (@[xche](https://github.com/xche))

- [Function] Fix the issue that reading metrics is always stuck in some cases.

    https://github.com/apache/pulsar/pull/9538 (@[315157973](https://github.com/315157973))

- [CI] CI Builds for WebSite and Mac OS write too much log ( due to missing the `-B` option).

    https://github.com/apache/pulsar/pull/9539 (@[eolivelli](https://github.com/eolivelli))

- [Function] Fix possible deadlock on broker-function service startup.

    https://github.com/apache/pulsar/pull/9499 (@[rdhabalia](https://github.com/rdhabalia))

- [Broker] Fix the metric data of `msgDelayed` for partitioned topics.

    https://github.com/apache/pulsar/pull/9529 (@[limingnihao](https://github.com/limingnihao))

- [C++] Remove namespace check from `MultiTopicsConsumerImpl`.

    https://github.com/apache/pulsar/pull/9520 (@[BewareMyPower](https://github.com/BewareMyPower))

- [TestClient] Fix logic in `ManagedLedgerWriter` when configuring `threadNum >= ledgerNum`.

    https://github.com/apache/pulsar/pull/9497 (@[WJL3333](https://github.com/WJL3333))

- [Broker] Fix the issue that when creating partition for an exist topic `RestException` is not thrown.

    https://github.com/apache/pulsar/pull/9342 (@[BewareMyPower](https://github.com/BewareMyPower))

- [CLI] Avoid duplicated options.

    https://github.com/apache/pulsar/pull/9469 (@[Renkai](https://github.com/Renkai))

- [CI] Fix duplicated canceling workflow runs.

    https://github.com/apache/pulsar/pull/9503 (@[potiuk](https://github.com/potiuk))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

### Blog / Article

- Migrate to Serverless with Pulsar Functions

    - https://streamnative.io/en/blog/tech/2021-02-10-migrate-to-serverless-with-pulsar-functions
