---
title: "2021-09-20-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-09-13 ~ 2021-09-19"
date: 2021-09-13 ~ 2021-09-19
description: "This is the Pulsar community weekly update for 2021-09-13 ~ 2021-09-19, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-09-20-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-09-13 ~ 2021-09-19

This is the Pulsar community weekly update for 2021-09-13 ~ 2021-09-19, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[freeznet](https://github.com/freeznet), [merlimat](https://github.com/merlimat), [yuruguo](https://github.com/yuruguo), [Shoothzj](https://github.com/Shoothzj),  [lhotari](https://github.com/lhotari), [codelipenghui](https://github.com/codelipenghui), [BewareMyPower](https://github.com/BewareMyPower), [aarondonwilliams](https://github.com/aarondonwilliams), [urfreespace](https://github.com/urfreespace), [michaeljmarshall](https://github.com/michaeljmarshall), [gaoran10](https://github.com/gaoran10), [dlg99](https://github.com/dlg99), [ravi-vaidyanathan](https://github.com/ravi-vaidyanathan), [hangc0276](https://github.com/hangc0276)


## Pulsar Program Overview
- Github Forks: 2.4k
- Github Stars: 9.6k
- Github Contributors: 448

## Pulsar Updates

### Highlights

- [Borker] PIP-45: Remove `ConfigurationCacheService` from `AuthorizationProvider`. 
<br>https://github.com/apache/pulsar/pull/12064 
by [merlimat](https://github.com/merlimat)

- [Broker] PIP-82: Add missing check for permissions on certain `ResourceGroup`. 
<br>https://github.com/apache/pulsar/pull/11957 
<br>by [ravi-vaidyanathan](https://github.com/ravi-vaidyanathan)

### Notable Features
- [Function] Pass `SubscriptionPosition` from `FunctionDetails` to `FunctionConfig` / `SinkConfig`. 
<br>https://github.com/apache/pulsar/pull/11831 
<br>by [freeznet](https://github.com/freeznet)

- [Broker] Improve logic for pausing replicated subscription snapshots when there is no traffic. 
<br>https://github.com/apache/pulsar/pull/11922 
<br>by [merlimat](https://github.com/merlimat)

- [Broker] Improve building `JwtParser`. 
<br>https://github.com/apache/pulsar/pull/12063 
<br>by [yuruguo](https://github.com/yuruguo)

- [Common] Use equals to compare string in `CmdGenerateDocs`. 
<br>https://github.com/apache/pulsar/pull/12061 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [Client] Force Python CI to use earlier version of Protobuf which supports Python2. 
<br>https://github.com/apache/pulsar/pull/12058 
<br>by [merlimat](https://github.com/merlimat)

- [BookKeeper] Avoid adding duplicated `BrokerEntryMetadata`. 
<br>https://github.com/apache/pulsar/pull/12018 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Broker] Optimize authz checks in `ServerCnx` when authz is not enabled.
<br>https://github.com/apache/pulsar/pull/12067 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

- [Broker] Refactor `PulsarResources` to avoid building metadata paths in matadata store. 
<br>https://github.com/apache/pulsar/pull/11693 
<br>by [merlimat](https://github.com/merlimat)

- [Proxy] Add new option `--num-messages` for a `consumer` and `reader` in pulsar-perf.
<br>https://github.com/apache/pulsar/pull/12016 
<br>by [yuruguo](https://github.com/yuruguo)

- [Connector] Add Debezium Source for Oracle. 
<br>https://github.com/apache/pulsar/pull/11520 
<br>by [dlg99](https://github.com/dlg99)

### Notable Bug Fix

- [Broker] Fix malformed string format. 
<br>https://github.com/apache/pulsar/pull/12060 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [Client] Fix endless `receiveAsync` loop in `MultiTopicsConsumer`.
<br>https://github.com/apache/pulsar/pull/12044 
<br>by [lhotari](https://github.com/lhotari)

- [Proxy] Fixed ProxyConnection to check the existence of auth_data field. 
<br>https://github.com/apache/pulsar/pull/12057 
<br>by [merlimat](https://github.com/merlimat)

- [Broker] Fix wrong key-hash selector used for new consumers after all the previous consumers are disconnected. 
<br>https://github.com/apache/pulsar/pull/12035 
<br>by [codelipenghui](https://github.com/codelipenghui)

- [Broker] Fix incorrect log placeholders. 
<br>https://github.com/apache/pulsar/pull/12014 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [C++] Remove Python3 from vcpkg.json. 
<br>https://github.com/apache/pulsar/pull/12092 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Build] Fix java-test-functions dependencies and packaging. 
<br>https://github.com/apache/pulsar/pull/10918 
<br>by [lhotari](https://github.com/lhotari)

## Events / News
- Upcoming Events
    - September 21-23th: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - September 30th: [Apache Pulsar Meetup Japan](https://japan-pulsar-user-group.connpass.com/event/222026/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)

- Call For Participation
    - [Pulsar Summit Asia 2021 CFP is Open until 09/30](https://pulsar.apache.org/blog/2021/08/18/asia-cfp/)