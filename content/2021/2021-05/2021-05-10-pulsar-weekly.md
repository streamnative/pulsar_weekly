---
title: "2021-05-10-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-05-03 ~ 2021-05-09"
date: 2021-05-03 ~ 2021-05-09
description: "This is the Pulsar community weekly update for 2021-05-03 ~ 2021-05-09, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-05-10-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-05-03 ~ 2021-05-09

This is the Pulsar community weekly update for 2021-05-03 ~ 2021-05-09, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [C++ Client] Avoid sending flow requests with zero permits.

  https://github.com/apache/pulsar/pull/10506 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Java Client] Avoid sending flow requests with zero permits.

  https://github.com/apache/pulsar/pull/10507 ([@BewareMyPower](https://github.com/BewareMyPower))

### Development

- [PIP-45] Revalidate the leader election after a session is recovered.

  https://github.com/apache/pulsar/pull/10457 ([@merlimat](https://github.com/merlimat))

### Notable Feature
  
- [Broker] Remove the residual information after forcibly deleting the namespace.

  https://github.com/apache/pulsar/pull/10465 ([@315157973](https://github.com/315157973))
  
- [Client] Fix the NPE in the Pulsar client.

  https://github.com/apache/pulsar/pull/10470 ([@abhilashmandaliya](https://github.com/abhilashmandaliya))
  
- [Bookie] Fix the issue that the publish callback's entry data is null during the ledger rollover.

  https://github.com/apache/pulsar/pull/10467 ([@BewareMyPower](https://github.com/BewareMyPower))
  
- [Enhancement] Improve the way to handle errors during localrun start-up process.

  https://github.com/apache/pulsar/pull/10450 ([@jerrypeng](https://github.com/jerrypeng))
  
- [Broker] The `readModifyUpdate` in the `MetadataCache` should return a `CompletableFuture<T>` with a newly applied value.

  https://github.com/apache/pulsar/pull/10474 ([@merlimat](https://github.com/merlimat))
  
- [Enhancement] Fix the possible memory leak of `TopicPolicies`.

  https://github.com/apache/pulsar/pull/10466 ([@315157973](https://github.com/315157973))
  
- [Consumer] Make the consumer thread safe and lock-free.

  https://github.com/apache/pulsar/pull/10352 ([@315157973](https://github.com/315157973))
  
- [Broker] Support `listenerName` for `HttpLookupService`.

  https://github.com/apache/pulsar/pull/10319 ([@315157973](https://github.com/315157973))
  
- [Bookie] Fix the potential bug in getting stats and the maximum number of topics per namespace and remove unnecessary error logs.

  https://github.com/apache/pulsar/pull/10500 ([@jerrypeng](https://github.com/jerrypeng))
  
- [Java Client] Fix the behavior of `Schema.AUTO_CONSUME()` with `KeyValueSchema` and write different versions of the schema.

  https://github.com/apache/pulsar/pull/10492 ([@eolivelli](https://github.com/eolivelli))
  
- [Broker] Add `onFilter` for the interceptor.

  https://github.com/apache/pulsar/pull/10489 ([@315157973](https://github.com/315157973))
  
- [Test] Remove the key_shared related tests from the quarantine group.

  https://github.com/apache/pulsar/pull/10508 ([@codelipenghui](https://github.com/codelipenghui))
  
### Notable Bug Fix

- [Broker] Add logging to `JavaInstanceRunnable` to help debug issues.

  https://github.com/apache/pulsar/pull/10461 ([@devinbost](https://github.com/devinbost))

- [Function] Fix the issue that the Pulsar Function API fails to use the authentication data to check the superuser.

  https://github.com/apache/pulsar/pull/10364 ([@zymap](https://github.com/zymap))

- [Client] Fix the issue that `hasMessageAvailableAsync` returns `true` but the message cannot be read.

  https://github.com/apache/pulsar/pull/10414 ([@315157973](https://github.com/315157973))

- [Broker] Fix the NPE in unblocking the stuck subscription task when the dispatcher is not created.

  https://github.com/apache/pulsar/pull/10430 ([@rdhabalia](https://github.com/rdhabalia))

- [Client] Fix the NPE in `GenericJsonRecord`.

  https://github.com/apache/pulsar/pull/10482 ([@abhilashmandaliya](https://github.com/abhilashmandaliya))

- [Broker] Fix the authorization error that is generated when the partition number of a partitioned topic is updated.

  https://github.com/apache/pulsar/pull/10333 ([@dragonls](https://github.com/dragonls))

- [Broker] Support `PolicyName` and `Authz` on new namespace routes.

  https://github.com/apache/pulsar/pull/7900 ([@KannarFr](https://github.com/KannarFr))

- [Offloader] Fix the AWS credentials usage issues.

  https://github.com/apache/pulsar/pull/8950 ([@KannarFr](https://github.com/KannarFr))

- [Pulsar-IO] Expose `SubscriptionType` in the `SinkContext`.

  https://github.com/apache/pulsar/pull/10446 ([@dlg99](https://github.com/dlg99))

- [Function] Fix the deadlock on monitoring the thread blocked by `LeaderService.isLeader()`.

  https://github.com/apache/pulsar/pull/10502 ([@freeznet](https://github.com/freeznet))

- [Function] Support setting custom configurations for the plugin worker service.

  https://github.com/apache/pulsar/pull/10504 ([@freeznet](https://github.com/freeznet))

- [Authz] Add granularity in the topic API authentication.

  https://github.com/apache/pulsar/pull/7523 ([@KannarFr](https://github.com/KannarFr))

### Event / News

- Pulsar Virtual Summit North America 2021

    - Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- Function Mesh - Simplify Complex Streaming Jobs in Cloud

  - https://streamnative.io/en/blog/release/2021-05-03-function-mesh-open-source