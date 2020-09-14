---
title: "2020-09-11-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-09-05 ~ 2020-09-11"
date: 2020-09-05 ~ 2020-09-11
description: "This is the Pulsar community weekly update for 2020-09-05 ~ 2020-09-11, with updates on Pulsar clients, transaction, Oauth2 authentication, Functions, security, and so on."
id: "2020-09-11-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-09-05 ~ 2020-09-11

This is the Pulsar community weekly update for 2020-09-05 ~ 2020-09-11, with updates on Pulsar clients, transaction, Oauth2 authentication, Functions, security, and so on.

### Development

- [Topic Policy] Support setting, getting, and removing `inactiveTopicPolicies` on the topic level.

    https://github.com/apache/pulsar/pull/7986 (@[315157973](https://github.com/315157973))

- [Bookie] Add `bookkeeperClientMinNumRacksPerWriteQuorum` and `bookkeeperClientEnforceMinNumRacksPerWriteQuorum` configuration options.

    https://github.com/apache/pulsar/pull/7977 (@[mkozioro](https://github.com/mkozioro))

- [Topic Policy] Support setting, getting, and removing `maxConsumers` on the topic level.

    https://github.com/apache/pulsar/pull/7968 (@[zhanghaou](https://github.com/zhanghaou))

- [Transaction] Update the transaction acknowledgement abort process on subscription.

    https://github.com/apache/pulsar/pull/7979 (@[gaoran10](https://github.com/gaoran10))

- [Topic Policy] Fix the overwritten order of `dispatchRate`.

    https://github.com/apache/pulsar/pull/8004 (@[315157973](https://github.com/315157973))

- [C++ Client] Support key-based batching for the C++ client.

    https://github.com/apache/pulsar/pull/7996 (@[BewareMyPower](https://github.com/BewareMyPower))

- [Pulsar Perf] Support setting the message key for consumers in the key-shared subscription mode.

    https://github.com/apache/pulsar/pull/7989 (@[315157973](https://github.com/315157973))

- [OAuth2] Get the Oauth2 token endpoint from the well-known configuration.

    https://github.com/apache/pulsar/pull/8006 (@[zymap](https://github.com/zymap))

- [Functions] Support specifying the sub position in Pulsar Functions.

    https://github.com/apache/pulsar/pull/7891 (@[wolfstudy](https://github.com/wolfstudy))

- [Topic Policy] Support setting, getting, and removing max consumers per subscription on the topic level.

    https://github.com/apache/pulsar/pull/8003 (@[hangc0276](https://github.com/hangc0276))

### Notable Bug Fix

- [Functions] Implement better error handling during close() of a batch source.

    https://github.com/apache/pulsar/pull/7984 (@[jerrypeng](https://github.com/jerrypeng))

- [Functions] Improve the batch source intermediate topic cleanup operation.

    https://github.com/apache/pulsar/pull/7985 (@[jerrypeng](https://github.com/jerrypeng))

- [Security] Upgrade the snakeyaml to verion 1.26.

    https://github.com/apache/pulsar/pull/7994 (@[wolfstudy](https://github.com/wolfstudy))

- [Broker] Avoid calculating the publish buffer of one ServerCnx multiple times when checking the broker's publish buffer.

    https://github.com/apache/pulsar/pull/7926 (@[aloyszhang](https://github.com/aloyszhang))

- [OAuth2] Fix the null exception when the proxy service is started with the OAuth2 authentication plugin.

    https://github.com/apache/pulsar/pull/8019 (@[zymap](https://github.com/zymap))

- [Broker] Fix `IndexOutOfBoundsException` in the Key_Shared subscription mode when messages are dispatched to consumers.

    https://github.com/apache/pulsar/pull/8024 (@[codelipenghui](https://github.com/codelipenghui))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

  - 09/09: "Apache Pulsar: Under the Hood for Java Developers" by Addison Higham in the Israeli Java Community (Java.IL)

    - Slides: https://docs.google.com/presentation/d/1zJdeFK9VVTDKL76UQimGWoJQOBlpEo5fmkGLbLh70GY/edit#slide=id.g944de4dcda_0_334
    - Video: https://www.youtube.com/watch?v=8DkZKsjjcG0&feature=youtu.be

### Blog / Article

- StreamNative Cloud - Getting Started

  -  https://streamnative.io/blog/tech/2020-09-10-streamnative-cloud-get-started