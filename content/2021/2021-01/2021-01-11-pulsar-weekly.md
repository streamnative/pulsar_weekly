---
title: "2021-01-11-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-01-04 ~ 2021-01-10"
date: 2021-01-04 ~ 2021-01-10
description: "This is the Pulsar community weekly update for 2021-01-04 ~ 2021-01-10, with updates on Pulsar client, broker, Functions, and so on."
id: "2021-01-11-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-01-04 ~ 2021-01-10

This is the Pulsar community weekly update for 2021-01-04 ~ 2021-01-10, with updates on Pulsar client, broker, Functions, and so on.

### Pulsar Highlight

Support the chained authentication with the same authentication method name. Therefore, users can configure multiple authentication providers with the same authentication method name.

by [@sijie](https://github.com/sijie)

### Development

- [PIP-45] Add `MetadataCache` implementation.

    https://github.com/apache/pulsar/pull/9148 [@merlimat](https://github.com/merlimat)

- [PIP-75] Replace the patched Google Protobuf with LightProto.

    https://github.com/apache/pulsar/pull/9046 [@merlimat](https://github.com/merlimat)

### Notable Feature

- [C++ Client] Add Advertised addresses lookup by `ListenerName` for the C++ client.

    https://github.com/apache/pulsar/pull/9119 by [@z2665](https://github.com/z2665)

- [Broker] Add `maxTopicsPerNamespace` limit for the namespace-level policy.

    https://github.com/apache/pulsar/pull/9042 [@hangc0276](https://github.com/hangc0276)

- [Pulsar] Enable spotbugs check in module `pulsar-common`.

    https://github.com/apache/pulsar/pull/9016 [@zymap](https://github.com/zymap)

- [Storage] Make the ledger rollover check task internal.

    https://github.com/apache/pulsar/pull/8946 [@hangc0276](https://github.com/hangc0276)

- [Stats] Add a new metric to monitor if the `mark-delete` position is advanced or not.

    https://github.com/apache/pulsar/pull/8930 [@sijie](https://github.com/sijie)

### Notable Bug Fix

- [Broker] Fix the issue that namespace-level policies return incorrect default values if no value is given by the user.

    https://github.com/apache/pulsar/pull/9149 [@315157973]https://github.com/315157973

- [Test] Resolve the race condition in `ManagedLedgerTest.testAsyncUpdateProperties()`.

    https://github.com/apache/pulsar/pull/9152 [@merlimat](https://github.com/merlimat)

- [pulsar-admin] Set `service-url` to false because `service-url` is not required for TLS-enabled clusters.

    https://github.com/apache/pulsar/pull/9127 [@dockerzhang]https://github.com/dockerzhang

- [Functions] Fix NPE in Go Functions if `BatchBuilder` is not set properly.

    https://github.com/apache/pulsar/pull/9124 [@flowchartsman]https://github.com/flowchartsman

- [Broker] Fix the issue that unloading namespaces bundle are blocked because `StampedLock` is not a reentrant and the `foreach` method of the `ConcurrentOpenHashMap` also acquires read lock.

    https://github.com/apache/pulsar/pull/9116 [@codelipenghui]https://github.com/codelipenghui

- [PulsarAdmin] Fix the issue that the `function-name` API returns the wrong type.

    https://github.com/apache/pulsar/pull/9115 [@tuteng]https://github.com/tuteng

- [Broker] Fix NPE when `MultiTopicsConsumerImpl` receives null-value messages.

    https://github.com/apache/pulsar/pull/9113 [@BewareMyPower]https://github.com/BewareMyPower

- [C++ Client] Fix the compilation issue caused by the non-virtual destructor.

    https://github.com/apache/pulsar/pull/9106 [@tongsucn](https://github.com/tongsucn)

- [Storage] Fix `BKIncorrectParameterException` in `ManagedLedgerInterceptorImpl`.

    https://github.com/apache/pulsar/pull/9091 [@aloyszhang](https://github.com/aloyszhang)

- [Broker] Fix `ConcurrentModificationException` when the Pulsar broker starts with KoP being enabled.

    https://github.com/apache/pulsar/pull/9088 [@aloyszhang](https://github.com/aloyszhang)

- [Broker] Fix the issue that the Pulsar broker expires one messages at a time after topics are unloaded.

    https://github.com/apache/pulsar/pull/9083 [@eolivelli]https://github.com/eolivelli

- [C++ Client] Fix the issue that the consumer sends `redeliverMessages` repeatedly.

    https://github.com/apache/pulsar/pull/9072 [@saosir](https://github.com/saosir)

- [Broker] Fix the issue that a wrong value is returned, when getting the partition metadata for a non-existing topic.

    https://github.com/apache/pulsar/pull/8818 [@aloyszhang](https://github.com/aloyszhang)

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Webinar] Watch Your Streams: Implementing OpenTelemetry with Apache Pulsar

    - https://us02web.zoom.us/webinar/register/3216003857537/WN_IyokJqHFRjicIuYT3ui4Ew

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq

### Blog / Article

- What's New in the Pulsar Flink Connector 2.7.0

    - https://flink.apache.org/2021/01/07/pulsar-flink-connector-270.html

- How Apache Pulsar is Helping Iterable Scale its Customer Engagement Platform

    - https://streamnative.io/en/blog/case/2021-01-05-iterable-scale-customer-engagement-platform-with-pulsar
