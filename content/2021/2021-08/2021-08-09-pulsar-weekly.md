---
title: "2021-08-09-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-08-02 ~ 2021-08-08"
date: 2021-08-02 ~ 2021-08-08
description: "This is the Pulsar community weekly update for 2021-08-02 ~ 2021-08-08, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-08-09-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-08-02 ~ 2021-08-08

This is the Pulsar community weekly update for 2021-08-02 ~ 2021-08-08, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: [codelipenghui](https://github.com/codelipenghui), [@Sunny-Island](https://github.com/Sunny-Island), [@gaoran10](https://github.com/gaoran10), [@Demogorgon314](https://github.com/Demogorgon314), [@Technoboy-](https://github.com/Technoboy-), [@frankxieke](https://github.com/frankxieke), [@urfreespace](https://github.com/urfreespace), [@lhotari](https://github.com/lhotari), [@315157973](https://github.com/315157973), [@aloyszhang](https://github.com/aloyszhang), [@HugoPelletier](https://github.com/HugoPelletier), [@MarvinCai](https://github.com/MarvinCai), [@massakam](https://github.com/massakam), [@WJL3333](https://github.com/WJL3333), [@equanz](https://github.com/equanz), [@freeznet](https://github.com/freeznet), [congbobo184](https://github.com/congbobo184),  [goldstar611](https://github.com/goldstar611), [galrose](https://github.com/galrose),  [tuteng](https://github.com/tuteng), [wuzhanpeng](https://github.com/wuzhanpeng), [liangyepianzhou](https://github.com/liangyepianzhou)

## Pulsar Program Overview
- Github Forks: 2.3K
- Github Stars: 9.4K
- Github Contributors: 434

## Pulsar Updates

### Pulsar Highlight

- [Schema] Replicate schemas across clusters, set the correct SchemaInfo for the replicated message and use
the `AutoProduceByte schema` for the producer of the replicator. 
<br>https://github.com/apache/pulsar/pull/11441
<br>by [codelipenghui](https://github.com/codelipenghui)
    

### Notable Feature

- [C++ Client] Simplify the implementation of getting the number of references from C++ client.
<br>https://github.com/apache/pulsar/pull/11535
<br>by [@Sunny-Island](https://github.com/Sunny-Island)

- [Python Client] Support Python schema type `Array`, `Map` to work with `Record`.
<br>https://github.com/apache/pulsar/pull/11530 
<br>by [@gaoran10](https://github.com/gaoran10)

- [Broker] Add additional servlet support to broker.
<br>https://github.com/apache/pulsar/pull/11498 
<br>by [@Demogorgon314](https://github.com/Demogorgon314)

- [Broker] Compress `ManagedLedgerInfo`.
<br>https://github.com/apache/pulsar/pull/11490 
<br>by [@gaoran10](https://github.com/gaoran10)

- [Broker] Add metrics `AddEntryWithReplicasBytesRate` for namespace.
<br>https://github.com/apache/pulsar/pull/11472 
<br>by [@Technoboy-](https://github.com/Technoboy-)

- [Broker] Add offload ledger info for admin topics stats
<br>https://github.com/apache/pulsar/pull/11465 
<br>by [@frankxieke](https://github.com/frankxieke)

- [Broker] Replicate schemas across clusters.
<br>https://github.com/apache/pulsar/pull/11441 
<br>by [@codelipenghui](https://github.com/codelipenghui)

- [Website][pulsar]: Generate docs for pulsar subcommand `websocket` automaticly.
<br>https://github.com/apache/pulsar/pull/11364 
<br>by [@urfreespace](https://github.com/urfreespace)

- [Website][pulsar]: Generate docs for pulsar subcommand `discovery` automaticly.
<br>https://github.com/apache/pulsar/pull/11358 
<br>by [@urfreespace](https://github.com/urfreespace)

- [Website][pulsar]: Generate docs for pulsar subcommand `initialize-cluster-metadata` automaticly.
<br>https://github.com/apache/pulsar/pull/11327 
<br>by [@urfreespace](https://github.com/urfreespace)

- [Website][pulsar]: Generate docs for pulsar subcommand `functions-worker` automaticly.
<br>https://github.com/apache/pulsar/pull/11326 
<br>by [@urfreespace](https://github.com/urfreespace)

- [Build] Use Ubuntu:20.04 base image for Pulsar docker images.
<br>https://github.com/apache/pulsar/pull/11026 
<br>by[@lhotari](https://github.com/lhotari)

### Notable Bug Fix

- [Broker] Fix the issue that all web threads get stuck when deleting the namespace.
<br>https://github.com/apache/pulsar/pull/11596 
<br>by [@315157973](https://github.com/315157973)

- [Java Client] Avoid creating new subscription name for reader if it's already configed.
<br>https://github.com/apache/pulsar/pull/11586 
<br>by [@aloyszhang](https://github.com/aloyszhang)

- [C++ Client] Fix wrong Base64 paddings.
<br>https://github.com/apache/pulsar/pull/11578 
<br>by [@BewareMyPower](https://github.com/BewareMyPower)

- [Broker] Introduce the backoff for setting to fix some topic policy operation.
<br>https://github.com/apache/pulsar/pull/11560 
<br>[@codelipenghui](https://github.com/codelipenghui)

- [Python Client] Check if the record is not `None`.
<br>https://github.com/apache/pulsar/pull/11559 
<br>by [@HugoPelletier](https://github.com/HugoPelletier)

- [C++/Python] Fix CI test bugs.
<br>https://github.com/apache/pulsar/pull/11557 
<br>by [@BewareMyPower](https://github.com/BewareMyPower)

- [Broker] Fix data lost when using earliest position to subscribe to a topic.
<br>https://github.com/apache/pulsar/pull/11547 
<br>by [@codelipenghui](https://github.com/codelipenghui)

- [Broker] Replace `orElse` with `orElseGet`.
<br>https://github.com/apache/pulsar/pull/11542 
<br>by [@Technoboy-](https://github.com/Technoboy-)

- [Broker] Fix time based backlog quota.
<br>https://github.com/apache/pulsar/pull/11509
<br>by [@MarvinCai](https://github.com/MarvinCai)

- [Python Client] Fix fields that are ignoring the required key argument.
<br>https://github.com/apache/pulsar/pull/11508 
<br>by [@HugoPelletier](https://github.com/HugoPelletier)

- [WebSocket] Make Query parameter `negativeAckRedeliveryDelay` effective even if DLQ is disabled.
<br>https://github.com/apache/pulsar/pull/11495 
<br>by [@massakam](https://github.com/massakam)

- [Java Client] Fix the issue that Consumer listener does not respect receiver queue size.
<br>https://github.com/apache/pulsar/pull/11455 ([@Technoboy-](https://github.com/Technoboy-))

- [Broker] `OffloadPoliciesImplBuilder` missing method and not implements `OffloadPolicies.Builder`.
<br>https://github.com/apache/pulsar/pull/11453 
<br>by [@WJL3333](https://github.com/WJL3333)

- [Broker] Fix producing messages when `preciseTopicPublishRateLimiterEnable=true`.
<br>https://github.com/apache/pulsar/pull/11442 
<br>by [@lhotari](https://github.com/lhotari)

- [Broker] Fixed the issue that Replicated Subscription doesn't replicate new subscription when remote producer is closed.
<br>https://github.com/apache/pulsar/pull/11382 
<br>by [@equanz](https://github.com/equanz)

- [Broker] Auth check `GetTopicsOfNamespace` with binary lookup service.
<br>https://github.com/apache/pulsar/pull/11172 
<br>by [@freeznet](https://github.com/freeznet)

- [Broker] Fix set-publish-rate when using `preciseTopicPublishRateLimiterEnable=true`.
<br>https://github.com/apache/pulsar/pull/10384 
<br>by [@lhotari](https://github.com/lhotari)

## Events / News

- Announcement
    - Welcome new Apache Pulsar PMC members, [Enrico Olivelli](https://github.com/eolivelli), [Lin Lin](https://github.com/315157973) and [Hang Chen](https://github.com/hangc0276)!
- Upcoming Events
    - August 11st: [August Pulsar Monthly Updates: A Deep Dive into Key-shared Subscription](https://streamnative.zoom.us/webinar/register/WN_BqHC8IUSSCCNiTO0OSjkdQ)
    - September 21-23rd: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)
- Call for Participation
    - [Pulsar Release Party in Guangzhou and Shenzhen, China](https://mp.weixin.qq.com/s/jacLGD1Vaaoe6bj2cD6lHQ)


## Credits
The Pulsar Weekly is brought to you by [gaoran10](https://github.com/gaoran10) and [Jipei Wang](https://github.com/JipeiWang)


Thank you for reading. See you next week!