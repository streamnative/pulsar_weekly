---
title: "2021-03-29-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-03-22 ~ 2021-03-28"
date: 2021-03-22 ~ 2021-03-28
description: "This is the Pulsar community weekly update for 2021-03-22 ~ 2021-03-28, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-03-29-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-03-22 ~ 2021-03-28

This is the Pulsar community weekly update for 2021-03-22 ~ 2021-03-28, with updates on Pulsar client, broker, transactions, and so on.

### Notable Feature

- [Broker] Support getting the applied compaction threshold.

    https://github.com/apache/pulsar/pull/10038 ([@315157973](https://github.com/315157973))

- [WebSocket] Support the `pong` logic in the WebSocket server.

    https://github.com/apache/pulsar/pull/10035 ([@linlinnn](https://github.com/linlinnn))

- [WebSocket] Allow the WebSocket proxy to consume and pass messages to the client without decryption.

    https://github.com/apache/pulsar/pull/10026 ([@rdhabalia](https://github.com/rdhabalia))

- [Authentication] Support the serializable stream-provider field in `AuthenticationTls`.

    https://github.com/apache/pulsar/pull/10020 ([@rdhabalia](https://github.com/rdhabalia

- [Client] Deal with partitioned-topic messages on different listener-threads.

    https://github.com/apache/pulsar/pull/10017 ([@rdhabalia](https://github.com/rdhabalia))

- [Kafka] Support `KeyValue` for `KafkaBytesSource`.

    https://github.com/apache/pulsar/pull/10002 ([@eolivelli](https://github.com/eolivelli))

- [Client] Support multiple topics for `MultiTopicsReaderImpl`.

    https://github.com/apache/pulsar/pull/9995 ([@315157973](https://github.com/315157973))

- [Pulsar SQL] Support querying the uppercase topics.

    https://github.com/apache/pulsar/pull/9980 ([@gaoran10](https://github.com/gaoran10))

- [Transactions] Clear aborted transactions from the transaction buffer.

    https://github.com/apache/pulsar/pull/9974 ([@congbobo184](https://github.com/congbobo184))

- [Pulsar-client] Add the command used to get the Pulsar version for Pulsar REST API, as well as the pulsar-admin and pulsar-client CLI tools.

    https://github.com/apache/pulsar/pull/9975 ([@tuteng](https://github.com/tuteng))

### Notable Bug Fix

- [Maven] Add `jersey-client` as the dependency of `pulsar-client-auth-sasl`.

    https://github.com/apache/pulsar/pull/10055 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Build] Fix possible name-mismatching bugs when building wheel files within the docker.

    https://github.com/apache/pulsar/pull/10051 ([@timmyyuan](https://github.com/timmyyuan))

- [Broker] Fix the incorrect time unit in updating `lastLedgerCreationInitiationTimestamp`.

    https://github.com/apache/pulsar/pull/10049 ([@wuzhanpeng](https://github.com/wuzhanpeng))

- [C++] Fix the issue that the paused zero-queue consumer still pre-fetches messages.

    https://github.com/apache/pulsar/pull/10036 ([@BewareMyPower](https://github.com/BewareMyPower))

- [C++] Support configuring debug-level logs simply.

    https://github.com/apache/pulsar/pull/10031 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Build] Fix shading for the `ahc-default.properties` file.

    https://github.com/apache/pulsar/pull/10007 ([@lhotari](https://github.com/lhotari))

- [C++] Fix the segmentation fault when getting the topic name from the received message ID.

    https://github.com/apache/pulsar/pull/10006 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Flaky test] Fix the `CurrentLedgerRolloverIfFullTest` flaky test.

    https://github.com/apache/pulsar/pull/10004 ([@lhotari](https://github.com/lhotari))

- [Client] Fix the useless retry when the maximum number of subscriptions is reached.

    https://github.com/apache/pulsar/pull/9991 ([@315157973](https://github.com/315157973))

- [Schema] Fix the NPE issue which is caused by the null value of SchemaInfo's properties.

    https://github.com/apache/pulsar/pull/9985 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Schema] Fix the `OutOfMemoryError` error which is caused by the topic with the schema KeyValue<GenericRecord, GenericRecord>.

    https://github.com/apache/pulsar/pull/9981 ([@eolivelli](https://github.com/eolivelli))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - 03/24: https://www.youtube.com/watch?v=JzExXJYiGvY