---
title: "2020-10-16-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-10-10 ~ 2020-10-16"
date: 2020-10-10 ~ 2020-10-16
description: "This is the Pulsar community weekly update for 2020-10-10 ~ 2020-10-16, with updates on Pulsar client, broker, Pulsar Functions, and so on."
id: "2020-10-16-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-10-10 ~ 2020-10-16

This is the Pulsar community weekly update for 2020-10-10 ~ 2020-10-16, with updates on Pulsar client, broker, Pulsar Functions, and so on.

### Development

- [Pulsar-client] Add the log level configuration in pulsar-client.

    https://github.com/apache/pulsar/pull/8195 (@[bbonnin](https://github.com/bbonnin))

- [Pulsar Client] Use `ThreadPoolExecutor` instead of `EventLoop` to improve system performance.

    https://github.com/apache/pulsar/pull/8208 (@[315157973](https://github.com/315157973))

- [Go Functions] Upgrade the Go client to version 0.2.0 for Go Functions.

    https://github.com/apache/pulsar/pull/8241 (@[wolfstudy](https://github.com/wolfstudy))

- [Pulsar Broker] Support limiting the publishing rate of topics at the broker level.

    https://github.com/apache/pulsar/pull/8235 (@[315157973](https://github.com/315157973))

- [Pulsar Broker] Support limiting the maximum number of tenants for each Pulsar cluster.

    https://github.com/apache/pulsar/pull/8261 (@[315157973](https://github.com/315157973))

- [Pulsar Broker] Support limiting the maximum number of namespaces for each tenant.

    https://github.com/apache/pulsar/pull/8267 (@[315157973](https://github.com/315157973))

- [Pulsar Broker] Add the read position in the consumer stats for preserving the dispatching order of messages.

    https://github.com/apache/pulsar/pull/8274 (@[codelipenghui](https://github.com/codelipenghui))

### Notable Bug Fix

- [Python] Limit enum34 installation via the environment markers.

    https://github.com/apache/pulsar/pull/8213 (@[languitar](https://github.com/languitar))

- [CPP Client] Fix some pending requests that are not completed when the Pulsar broker is closed.

    https://github.com/apache/pulsar/pull/8232 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Pulsar Broker] Modify the occasion used for triggering listeners.

    https://github.com/apache/pulsar/pull/8234 (@[315157973](https://github.com/315157973))

- [Pulsar Broker] Fix stuck lookup operations when the Pulsar broker is starting up.

    https://github.com/apache/pulsar/pull/8273 (@[merlimat](https://github.com/merlimat))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

  - Low-Latency Stream Processing with Jet
    
    https://us02web.zoom.us/webinar/register/3216003857537/WN_821OFj6ITN23Y8uf8KgEag
    
  - Flink + Pulsar: The Path To Unified Batch and Streaming - Addison Higham

    https://www.flink-forward.org/global-2020/conference-program#flink---pulsar--the-path-to-unified-batch-and-streaming-

### Blog / Article

- 10 Reasons to Choose Apache Pulsar Over Apache Kafka - Maximilian Michels

  - https://dzone.com/articles/10-reasons-to-choose-apache-pulsar-over-apache-kaf
