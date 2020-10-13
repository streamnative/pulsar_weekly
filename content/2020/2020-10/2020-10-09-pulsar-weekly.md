---
title: "2020-10-09-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-09-26 ~ 2020-10-09"
date: 2020-09-26 ~ 2020-10-09
description: "This is the Pulsar community weekly update for 2020-09-26 ~ 2020-10-09, with updates on Pulsar client, broker, Pulsar Admin, Pulsar Functions, Pulsar schema, and so on."
id: "2020-10-09-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-09-26 ~ 2020-10-09

This is the Pulsar community weekly update for 2020-09-26 ~ 2020-10-09, with updates on Pulsar client, broker, Pulsar Admin, Pulsar Functions, Pulsar schema, and so on.

### Development

- [Client] Improve timeout handling in ClientCnx to cover all remaining request types that do not handle timeout.

    https://github.com/apache/pulsar/pull/8149 (@[lhotari](https://github.com/lhotari))

- [Broker] Intercept messages sent to consumers and support throwing interception exceptions.

    https://github.com/apache/pulsar/pull/8129 (@[zymap](https://github.com/zymap))

- [pulsar-admin] Support deleting data associated with a cluster.

    https://github.com/apache/pulsar/pull/8133 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Broker] Skip intercepting multipart requests.

    https://github.com/apache/pulsar/pull/8156 (@[zymap](https://github.com/zymap))

- [Common] Support specifying multiple IPv6 host addresses in `brokerServiceUrl`.

    https://github.com/apache/pulsar/pull/8120 (@[wangjialing218](https://github.com/wangjialing218))

- [Broker] Add `getLastMessageId` Pulsar Admin API (V1).

    https://github.com/apache/pulsar/pull/8081 (@[rdhabalia](https://github.com/rdhabalia))

- [pulsar-admin] Add the CLI command to get the last message ID.

    https://github.com/apache/pulsar/pull/8082 (@[rdhabalia](https://github.com/rdhabalia))

- [Admin] Support deleting schema ledgers when deleting topics.

    https://github.com/apache/pulsar/pull/8167 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Broker] Add the command used for deleting the cluster metadata from ZooKeeper.

    https://github.com/apache/pulsar/pull/8169 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Functions] Support disabling to forward source message properties.

    https://github.com/apache/pulsar/pull/8158 (@[zymap](https://github.com/zymap))

- [Broker] Support disabling replicated subscriptions.

    https://github.com/apache/pulsar/pull/8144 (@[k2la](https://github.com/k2la))

- [Common] Add `ChannelFutures` utility class to `CompletableFuture`.

    https://github.com/apache/pulsar/pull/8137 (@[racorn](https://github.com/racorn))

- [Broker] Check the null point before setting auto-read.

    https://github.com/apache/pulsar/pull/7999 (@[yuanboliu](https://github.com/yuanboliu))

- [Python Client] Update the script used for building the docker images to make the Python client work.

    https://github.com/apache/pulsar/pull/8153 (@[massakam](https://github.com/massakam))

- [IO] Add the `org.apache.pulsar.io.core.Context` interface.

    https://github.com/apache/pulsar/pull/8164 (@[david-streamlio](https://github.com/david-streamlio))

- [Client] Support using SNI for the TLS-enabled Pulsar Java broker client.

    https://github.com/apache/pulsar/pull/8117 (@[racorn](https://github.com/racorn))

- [Admin] Support getting the ledger metadata along with internal stats of topics.

    https://github.com/apache/pulsar/pull/8180 (@[rdhabalia](https://github.com/rdhabalia))

- [Broker] Add a new state for the namespace-level TTL.

    https://github.com/apache/pulsar/pull/8178 (@[315157973](https://github.com/315157973))

- [Python Client] Expose the `batchingType` interface.

    https://github.com/apache/pulsar/pull/8185 (@[hangc0276](https://github.com/hangc0276))

- [Broker] Clean inactive non-persistent subscriptions.

    https://github.com/apache/pulsar/pull/8166 (@[315157973](https://github.com/315157973))

- [Topic Policy] Support null check to avoid the NPE for `internalSetTopicPolicies`.

    https://github.com/apache/pulsar/pull/8201 (@[hangc0276](https://github.com/hangc0276))

- [C++ Client] Add an epoch for C++ client `HandleBase` to handle the timeout issue when creating the producer.

    https://github.com/apache/pulsar/pull/8191 (@[hangc0276](https://github.com/hangc0276))

- [Dashboard] Fix the `consumerName` migration issue in the Django model of the Pulsar dashboard.

    https://github.com/apache/pulsar/pull/8188 (@[sbourkeostk](https://github.com/sbourkeostk))

- [Go Client] Fix the argument type of `pulsarProducerSendCallbackProxy`.

    https://github.com/apache/pulsar/pull/8186 (@[massakam](https://github.com/massakam))

- [Functions] Propagate user-defined parameters into instances of Pulsar Go functions.

    https://github.com/apache/pulsar/pull/8132 (@[vaihtovirta](https://github.com/vaihtovirta))

- [Bookie] Expose `ensemblePlacementPolicy` in `bookkeeper.conf`.

    https://github.com/apache/pulsar/pull/8210 (@[hangc0276](https://github.com/hangc0276))

- [Broker] Enable intercepting filters only when interceptors are configured.

    https://github.com/apache/pulsar/pull/8157 (@[zymap](https://github.com/zymap))

- [Python Client] Add default values for Python schema fields.

    https://github.com/apache/pulsar/pull/8122 (@[hangc0276](https://github.com/hangc0276))

### Notable Bug Fix

- [C++ Client] Fix the unstable unit test of `testIndividualAck`.

    https://github.com/apache/pulsar/pull/8141 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Client] Fix `ConsumerImpl` memory leaks.

    https://github.com/apache/pulsar/pull/8160 (@[lhotari](https://github.com/lhotari))

- [Broker] Fix error codes returned to the Pulsar client when the service unit is not ready.

    https://github.com/apache/pulsar/pull/8147 (@[massakam](https://github.com/massakam))

- [Schema] Fix the possible NPE when starting `BookkeeperSchemaStorage`.

    https://github.com/apache/pulsar/pull/8172 (@[MaiCw4J](https://github.com/MaiCw4J))

- [Admin] Fix the issue of failing to peek messages when the subscription name does not exist.

    https://github.com/apache/pulsar/pull/8182 (@[hangc0276](https://github.com/hangc0276))

- [Client] Fix the issue that the paused consumer receives new messages when reconnecting to the broker.

    https://github.com/apache/pulsar/pull/8165 (@[massakam](https://github.com/massakam))

- [Broker] Fix the exception that is thrown when closing the Pulsar service.

    https://github.com/apache/pulsar/pull/8197 (@[hangc0276](https://github.com/hangc0276))

- [Schema] Fix the issue that JSON schema deserializes bytes to strings.

    https://github.com/apache/pulsar/pull/8140 (@[hangc0276](https://github.com/hangc0276))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [ApacheCon] ApacheCon @Home 2020

    - All video recordings are available at [here](https://www.youtube.com/playlist?list=PLU2OcwpQkYCy_awEe5xwlxGTk5UieA37m).

- [Training]

  - Broker Routing

    https://www.youtube.com/watch?v=f7nVSxeZD2M

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

  - Low-Latency Stream Processing with Jet
    
    https://us02web.zoom.us/webinar/register/3216003857537/WN_821OFj6ITN23Y8uf8KgEag
    
  - Flink + Pulsar: The Path To Unified Batch and Streaming - Addison Higham

    https://www.flink-forward.org/global-2020/conference-program#flink---pulsar--the-path-to-unified-batch-and-streaming-

### Blog / Article

- Building An Event-Driven Orchestration Engine - Gilles Barbier

  - https://medium.com/@gillesbarbier/building-an-event-driven-orchestration-engine-bf62d45aef5d

- Pulsar Function Deep Dive - Sanjeev Kulkarni

  - https://streamnative.io/blog/tech/2020-10-06-pulsar-functions-deep-dive