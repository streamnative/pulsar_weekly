---
title: "2021-06-28-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-06-21 ~ 2021-06-27"
date: 2021-06-21 ~ 2021-06-27
description: "This is the Pulsar community weekly update for 2021-06-21 ~ 2021-06-27, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-06-28-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-06-21 ~ 2021-06-27

This is the Pulsar community weekly update for 2021-06-21 ~ 2021-06-27, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [Topic Policy] Fix potential data lost on the system topic when topic compaction is not triggered yet.

    https://github.com/apache/pulsar/pull/11003 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Add the resource-group configuration listener.

    https://github.com/apache/pulsar/pull/10657 ([@bharanic-dev](https://github.com/bharanic-dev))

### Development

- [PIP-82] [Broker] Add the resource-group configuration listener.

    https://github.com/apache/pulsar/pull/10657 ([@bharanic-dev](https://github.com/bharanic-dev))

### Notable Feature

- [Security] Upgrade Vertx to version 3.9.8 to address vulnerability CVE-2019-17640.

    https://github.com/apache/pulsar/pull/10889 ([@lhotari](https://github.com/lhotari))

- [Security] Upgrade Commons Codec to version 1.15.

    https://github.com/apache/pulsar/pull/10864 ([@lhotari](https://github.com/lhotari))

- [Build] Change the NAR package name for `pulsar-io-kafka-connect-adaptor`.

    https://github.com/apache/pulsar/pull/10976 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Avoid exposing meaningless stats for the consumer.

    https://github.com/apache/pulsar/pull/11005 ([@codelipenghui](https://github.com/codelipenghui))

- [Tests] Convert JUnit tests to TestNG.

    https://github.com/apache/pulsar/pull/11020 ([@lhotari](https://github.com/lhotari))

- [Admin] Exclude the system topic in the `maxTopicsPerNamespace` check.

    https://github.com/apache/pulsar/pull/10850 ([@yangl](https://github.com/yangl))

- [Proxy] Limit the replay buffer size in `AdminProxyHandler`.

    https://github.com/apache/pulsar/pull/10944 ([@lhotari](https://github.com/lhotari))

- [Schema Registry] Make `KeyValueSchema` and the `AutoConsume` component work even when the schema is not set on the topic.

    https://github.com/apache/pulsar/pull/10995 ([@eolivelli](https://github.com/eolivelli))

- [Tests] Add a test for `TopicCountEquallyDivideBundleSplitAlgorithm`.

    https://github.com/apache/pulsar/pull/11015 ([@mattisonchao](https://github.com/mattisonchao))

- [Functions] Reorganize the context hierarchy for Pulsar Functions.

    https://github.com/apache/pulsar/pull/10631 ([@nlu90](https://github.com/nlu90))

- [Tests] Use TestNG instead of JUnit for tests.

    https://github.com/apache/pulsar/pull/11027 ([@315157973](https://github.com/315157973))

- [Python Functions] Use the keyword argument to create `pulsar_client`.

    https://github.com/apache/pulsar/pull/11080 ([@freeznet](https://github.com/freeznet))

- [Python Functions] Use the subscription name defined in Function details.

    https://github.com/apache/pulsar/pull/11076 ([@lhotari](https://github.com/lhotari))

- [Broker] Print the message metadata when getting messages by the message ID.

    https://github.com/apache/pulsar/pull/11092 ([@codelipenghui](https://github.com/codelipenghui))

- [C++ and Python] Add the connection timeout configuration.

    https://github.com/apache/pulsar/pull/11029 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Security] Exclude the `grpc-okhttp` dependency and set the OkHttp3 and Okio versions.

    https://github.com/apache/pulsar/pull/11025 ([@lhotari](https://github.com/lhotari))

- [Authorization] Remove the ternary operation and correct `brokerClientAuthenticationParameter`.

    https://github.com/apache/pulsar/pull/11090 ([@Technoboy-](https://github.com/Technoboy-))

- [Configuration] Add missing configuration entries.

    https://github.com/apache/pulsar/pull/11095 ([@junquero](https://github.com/junquero))

### Notable Bug Fix

- [Client] Fix the `NoClassDefFoundError` that the `io.airlift.compress.lz4.UnsafeUtil` class cannot be initialized.

    https://github.com/apache/pulsar/pull/10983 ([@newur](https://github.com/newur))

- [Functions] Include the Common-IO in the Java Function instance.

    https://github.com/apache/pulsar/pull/10939 ([@bharanic-dev](https://github.com/bharanic-dev))

- [Broker] Fix the issue that occurs when creating partitioned topics in the replicated namespace.

    https://github.com/apache/pulsar/pull/10963 ([@gaoran10](https://github.com/gaoran10))

- [Broker] Fix the backlog issue cause by the `--precise-backlog=true` parameter.

    https://github.com/apache/pulsar/pull/10966 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Fix the incorrect port of the `advertisedListener`.

    https://github.com/apache/pulsar/pull/10961 ([@315157973](https://github.com/315157973))

- [Tests] Fix the `testEnableAndDisableTopicDelayedDelivery` Flaky test.

    https://github.com/apache/pulsar/pull/11009 ([@315157973](https://github.com/315157973))

- [Client] Release `multiTopicsConsumerImpl` when unsubscribing topics.

    https://github.com/apache/pulsar/pull/10997 ([@Shoothzj](https://github.com/Shoothzj))

- [Tests] Fix the `ManagedLedgerTest` Flaky test.

    https://github.com/apache/pulsar/pull/11016 ([@codelipenghui](https://github.com/codelipenghui))

- [Topic Policy] Fix potential data lost on the system topic when topic compaction is not triggered yet.

    https://github.com/apache/pulsar/pull/11003 ([@codelipenghui](https://github.com/codelipenghui))

- [Tests] Fix the `PrimitiveSchemaTest` Flaky test.

    https://github.com/apache/pulsar/pull/11038 ([@eolivelli](https://github.com/eolivelli))

- [Tests] Fix the `AdminApiTest` Flaky test.

    https://github.com/apache/pulsar/pull/11039 ([@hangc0276](https://github.com/hangc0276))

- [Transaction] Fix the issue that the broker initializes transaction-related topics when loading namespace bundles.

    https://github.com/apache/pulsar/pull/11022 ([@congbobo184](https://github.com/congbobo184))

- [Tests] Fix the issue that the `assertEquals` method's parameter order is changed when changing from JUnit to TestNG.

    https://github.com/apache/pulsar/pull/11035 ([@hangc0276](https://github.com/hangc0276))

- [Tests] Fix the `AdminApiOffloadTest` Flaky test.

    https://github.com/apache/pulsar/pull/11028 ([@hangc0276](https://github.com/hangc0276))

- [Tests] Fix the `ResourceGroupConfigListenerTest` Flaky test.

    https://github.com/apache/pulsar/pull/11048 ([@lhotari](https://github.com/lhotari))

- [Python] Fix the error in importing the Pulsar 2.8.0 Python client when AvroSchema is not used.

    https://github.com/apache/pulsar/pull/11034 ([@merlimat](https://github.com/merlimat))

- [Tests] Fix the `AdminApiTest` Flaky test.

    https://github.com/apache/pulsar/pull/11059 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker] Make the `PulsarClusterMetadataTeardown` deletions idempotent.

    https://github.com/apache/pulsar/pull/11042 ([@merlimat](https://github.com/merlimat))

- [C++] Fix the issue that the C++ source code is compiled unsuccessfully for Windows 32-bit build.

    https://github.com/apache/pulsar/pull/11082 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Tests] Fix the `testTransactionMetaStoreAssignAndFailover` Flaky test.

    https://github.com/apache/pulsar/pull/11073 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker] Fix the incorrectly-used loggers.

    https://github.com/apache/pulsar/pull/11047 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker] Add the authoritative flag for the topic-level policy to avoid the redirect loop.

    https://github.com/apache/pulsar/pull/11051 ([@codelipenghui](https://github.com/codelipenghui))

- [Test] Fix the `testDuplicateConcurrentSubscribeCommand` Flaky test.

    https://github.com/apache/pulsar/pull/11089 ([@hangc0276](https://github.com/hangc0276))

- [C++] Fix the issue that the `KeySharedMeta` is not set as a subscribe command.

    https://github.com/apache/pulsar/pull/11088 ([@k2la](https://github.com/k2la))

- [Topic Policy] Fix the issue that the topic-level retention policy does not work.

    https://github.com/apache/pulsar/pull/11021 ([@hangc0276](https://github.com/hangc0276))

- [Functions] Fix the build failure caused by the SpotBugs.

    https://github.com/apache/pulsar/pull/10792 ([@Jason918](https://github.com/Jason918))

- [Build] Fix the compilation error caused by the number of incorrect parameters.

    https://github.com/apache/pulsar/pull/11104 ([@mattisonchao](https://github.com/mattisonchao))

- [Broker] Fix the issue that the response filter processes asynchronous responses incorrectly.

    https://github.com/apache/pulsar/pull/11052 ([@gaoran10](https://github.com/gaoran10))

- [Topic Policy] Fix the `SystemTopicBasedTopicPoliciesService` race condition.

    https://github.com/apache/pulsar/pull/11097 ([@codelipenghui](https://github.com/codelipenghui))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

  - Introduction to Apache Pulsar EP05

    - 06/23: https://www.youtube.com/watch?v=rWfPFsga3Qk

### Blog / Article

- Pulsar Hackathon 2021 Winners Announced

    - https://streamnative.io/en/blog/community/2021-06-22-pulsar-hackathon-2021-winners-announced

- Highlights from The Pulsar Virtual Summit North America 2021

    - https://streamnative.io/en/blog/community/2021-06-22-highlights-from-the-pulsar-virtual-summit-north-america-2021
