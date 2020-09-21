---
title: "2020-09-18-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-09-12 ~ 2020-09-18"
date: 2020-09-12 ~ 2020-09-18
description: "This is the Pulsar community weekly update for 2020-09-12 ~ 2020-09-18, with updates on Pulsar client, broker, transaction, bookie, security, and so on."
id: "2020-09-18-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-09-12 ~ 2020-09-18

This is the Pulsar community weekly update for 2020-09-12 ~ 2020-09-18, with updates on Pulsar client, broker, transaction, bookie, security, and so on.

### Development

- [Transaction] Support the pending-ack state for batch messages.

    https://github.com/apache/pulsar/pull/8037(@[congbobo184](https://github.com/congbobo184))

- [Pulsar Broker] Support configuring the basic rate limiting for HTTP requests.

    https://github.com/apache/pulsar/pull/8031 (@[merlimat](https://github.com/merlimat))

- [Bookie] Update the BookKeeper's `main` method class.

    https://github.com/apache/pulsar/pull/8065 (@[hrsakai](https://github.com/hrsakai ))

- [Bouncy Castle] Upgrade Bouncy Castle to the newest version.

    https://github.com/apache/pulsar/pull/8047 (@[srkukarni](https://github.com/srkukarni))

### Notable Bug Fix

- [Security]  Avoid re-connecting to the server if the client fails to be authenticated.

    https://github.com/apache/pulsar/pull/8058 (@[zymap](https://github.com/zymap))

- [Transaction] Fix the transaction message acknowledgement issue.

    https://github.com/apache/pulsar/pull/8007 (@[gaoran10](https://github.com/gaoran10))

- [Pulsar Client] Use `tlsEnableHostnameVerification` for `ClientBuilder` in `PulsarClientTool`.

    https://github.com/apache/pulsar/pull/8041 (@[aahmed-se](https://github.com/aahmed-se))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

  - Low-Latency Stream Processing with Jet

    https://us02web.zoom.us/webinar/register/3216003857537/WN_821OFj6ITN23Y8uf8KgEag

### Blog / Article

- Pulsar Flink Connector 2.5.0

  - https://streamnative.io/blog/release/2020-09-17-pulsar-flink-connector-250