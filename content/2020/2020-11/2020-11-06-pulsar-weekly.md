---
title: "2020-11-06-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-10-31 ~ 2020-11-06"
date: 2020-10-31 ~ 2020-11-06
description: "This is the Pulsar community weekly update for 2020-10-31 ~ 2020-11-06, with updates on Pulsar client, broker, transaction, WebSocket, tiered storage, and so on."
id: "2020-11-06-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-10-31 ~ 2020-11-06

This is the Pulsar community weekly update for 2020-10-31 ~ 2020-11-06, with updates on Pulsar client, broker, transaction, WebSocket, tiered storage, and so on.

### Pulsar Highlight

Support Azure BlobStore offload configuration. Pulsar supports using `Azure` to offload data. For details, see [PR-8436](https://github.com/apache/pulsar/pull/8436).

by ([@gaoran10](https://github.com/gaoran10))

### Notable Feature

- [Broker] Get the list of bundles under a namespace.

    https://github.com/apache/pulsar/pull/8450 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Unset the offload policies for namespaces.

    https://github.com/apache/pulsar/pull/8446 ([@Renkai](https://github.com/Renkai))

- [WebSocket] Add the redelivery count property to messages delivered through the WebSocket service.

    https://github.com/apache/pulsar/pull/8074 ([@IvanStoilov](https://github.com/IvanStoilov))

- [Tiered Storage] Support AWS credentials based on offload policies.

    https://github.com/apache/pulsar/pull/7950 ([@KannarFr](https://github.com/KannarFr))

- [Transaction] Support producing batch transaction messages.

    https://github.com/apache/pulsar/pull/8415 ([@gaoran10](https://github.com/gaoran10))

- [Tiered Storage] Support Azure BlobStore offload configuration.

    https://github.com/apache/pulsar/pull/8436 ([@gaoran10](https://github.com/gaoran10))

- [Broker] Start the `ml-add-ops` latency timer when the `bk-add` entry request initiates to capture the managed-ledger add-latency.

    https://github.com/apache/pulsar/pull/4419 ([@rdhabalia](https://github.com/rdhabalia))

### Notable Bug Fix

- [Broker] Fix the issue that the bookie-isolation placement-policy does not configuring the rackaware policy.

    https://github.com/apache/pulsar/pull/8461 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Fix the ZooKeeper cache expiration check.

    https://github.com/apache/pulsar/pull/8458 ([@hrsakai](https://github.com/hrsakai))

- [Proxy] Add the error log for the Pulsar proxy starter.

    https://github.com/apache/pulsar/pull/8451 ([@gaoran10](https://github.com/gaoran10))

- [Proxy] Ensure to pass 0 to the `ByteArrayOutputStreame` argument if `request.getContentLength()` returns a negative number.

    https://github.com/apache/pulsar/pull/8448 ([@magrain](https://github.com/magrain))

- [Function] Fix the returned status code for getting Function state when the Function state does not exist.

    https://github.com/apache/pulsar/pull/8437 ([@jerrypeng](https://github.com/jerrypeng))

- [Client] Fix the `AutoUpdatePartitionsInterval` setting problem.

    https://github.com/apache/pulsar/pull/8227 ([@RobertIndie](https://github.com/RobertIndie))

- [Broker] Fix the hash collision in the Key_Shared subscription mode.

    https://github.com/apache/pulsar/pull/8396 ([@ltamber](https://github.com/ltamber))

- [C++ Client] Allow to configure Key_Shared with out-of-order delivery.

    https://github.com/apache/pulsar/pull/7842 ([@merlimat](https://github.com/merlimat))

- [Client] Fix the `AutoUpdatePartitionsInterval` setting.

    https://github.com/apache/pulsar/pull/8227 ([@RobertIndie](https://github.com/RobertIndie))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020