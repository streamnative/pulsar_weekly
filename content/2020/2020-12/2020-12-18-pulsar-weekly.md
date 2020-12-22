---
title: "2020-12-18-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-12-12 ~ 2020-12-18"
date: 2020-12-12 ~ 2020-12-18
description: "This is the Pulsar community weekly update for 2020-12-12 ~ 2020-12-18, with updates on Pulsar client, broker, Functions, and so on."
id: "2020-12-18-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-12-12 ~ 2020-12-18

This is the Pulsar community weekly update for 2020-12-12 ~ 2020-12-18, with updates on Pulsar client, broker, Functions, and so on.

### Pulsar Highlight

- [Java Client] Implement the memory limit enforcement for the producer.

    https://github.com/apache/pulsar/pull/8965 ([@merlimat](https://github.com/merlimat))

- [Java Client] Support the `WaitForExclusive` access mode for the producer.

    https://github.com/apache/pulsar/pull/8992 ([@merlimat](https://github.com/merlimat))

- [Broker] Introduce the lightweight broker entry metadata.

    https://github.com/apache/pulsar/pull/8618 ([@aloyszhang](https://github.com/aloyszhang))

### Notable Feature

- [Schema] Add default values for properties in SchemaInfoBuilder.

    https://github.com/apache/pulsar/pull/8952 ([@jianyun8023](https://github.com/jianyun8023))

- [KoP] Support updating stats with specified stats.

    https://github.com/apache/pulsar/pull/8951 ([@dockerzhang](https://github.com/dockerzhang))

- [Broker] Support configuring the maximum number of subscriptions per topic on the topic level.

    https://github.com/apache/pulsar/pull/8948 ([@315157973](https://github.com/315157973))

- [Websocket] Support `deliverAt` and `deliverAfter` attributes for the WebSocket producer.

    https://github.com/apache/pulsar/pull/8945 ([@MarvinCai](https://github.com/MarvinCai))

- [Broker] Support limiting the maximum number of topics per namespace.

    https://github.com/apache/pulsar/pull/8942 ([@hangc0276](https://github.com/hangc0276))

- [Broker] Expose the non-contiguous deleted message range stats.

    https://github.com/apache/pulsar/pull/8936 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Add the `beforeSendMessage` method to intercept entries before sending them to consumers.

    https://github.com/apache/pulsar/pull/8932 ([@sijie](https://github.com/sijie))

- [Broker] Support configuring the maximum number of subscriptions per topic on the namespace level.

    https://github.com/apache/pulsar/pull/8924 ([@315157973](https://github.com/315157973))

- [C++ Client] Add consumer's configurations for the reader to decrypt encrypted messages.

    https://github.com/apache/pulsar/pull/8905 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Functions] Provide an interface for the Functions worker service.

    https://github.com/apache/pulsar/pull/8560 ([@sijie](https://github.com/sijie))

### Notable Bug Fix

- [Java Client] Fix the NPE when the Pulsar client receives acknowledgement for published messages from a closed producer.

    https://github.com/apache/pulsar/pull/8979 ([@rdhabalia](https://github.com/rdhabalia))

- [Admin] Fix the `AdminApiTest2.testMaxSubPerTopicApi` Flaky test.

    https://github.com/apache/pulsar/pull/8970 ([@315157973](https://github.com/315157973))

- [Broker] Fix the NPE in `PersistentStickyKeyDispatcherMultipleConsumers`.

    https://github.com/apache/pulsar/pull/8969 ([@315157973](https://github.com/315157973))

- [Broker] Clean up topics that fail to be unloaded from the cache.

    https://github.com/apache/pulsar/pull/8968 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Update the Maven artifact version.

    https://github.com/apache/pulsar/pull/8966 ([@aahmed-se](https://github.com/aahmed-se))

- [Broker] Fix the metadata setup compatibility issue.

    https://github.com/apache/pulsar/pull/8959 ([@zymap](https://github.com/zymap))

- [Broker] Fix the issue that the subscription dispatching rate fails to work after topics are unloaded without a dispatching rate limit.

    https://github.com/apache/pulsar/pull/8947 ([@codelipenghui](https://github.com/codelipenghui))

- [Pulsar IO] Fix the file name of the `pulsar-io.yaml` file and the `sourceConfigClass` class.

    https://github.com/apache/pulsar/pull/8941 ([@flowchartsman](https://github.com/flowchartsman))

- [Schema] Fix the issue that the customized Avro schema does not work for the consumer.

    https://github.com/apache/pulsar/pull/8939 ([@reswqa](https://github.com/reswqa))

- [Broker] Fix the project style error in Pulsar broker.

    https://github.com/apache/pulsar/pull/8933 ([@zsh0139](https://github.com/zsh0139))

- [Java Client] Add more information in sending `TimeoutException` for troubleshooting.

    https://github.com/apache/pulsar/pull/8931 ([@sijie](https://github.com/sijie))

- [Pulsar CI] Disable Maven's HTTP connection pooling by passing the `-Dhttp.keepAlive=false -Dmaven.wagon.http.pool=false in MAVEN_OPTS` environment variable.

    https://github.com/apache/pulsar/pull/8921 ([@lhotari](https://github.com/lhotari))

- [Pulsar Build] Use absolute path to locate license and checkstyle plugin configurations.

    https://github.com/apache/pulsar/pull/8918 ([@lhotari](https://github.com/lhotari))

- [Pulsar Client] Fix the issue that the `authParams` parameter shows in the log with secret string(*****).

    https://github.com/apache/pulsar/pull/8910 ([@hangc0276](https://github.com/hangc0276))

- [Pulsar Package] Fix the issue that the package fails to be uploaded.

    https://github.com/apache/pulsar/pull/8907 ([@zymap](https://github.com/zymap))

- [Java Shade Client] Add the encryption integration test.

    https://github.com/apache/pulsar/pull/8850 ([@RobertIndie](https://github.com/RobertIndie))


### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq

### Blog / Article

- Using Apache Pulsar With Kotlin -- Gilles Barbier

    - https://gillesbarbier.medium.com/using-apache-pulsar-with-kotlin-3b0ab398cf52