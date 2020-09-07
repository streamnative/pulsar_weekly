---
title: "2020-09-04-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-08-29 ~ 2020-09-04"
date: 2020-08-29 ~ 2020-09-04
description: "This is the Pulsar community weekly update for 2020-08-29 ~ 2020-09-04, with updates on Pulsar clients, brokers, and so on."
id: "2020-09-04-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-08-29 ~ 2020-09-04

This is the Pulsar community weekly update for 2020-08-29 ~ 2020-09-04, with updates on Pulsar transaction, broker, metrics and so on.

### Development

- [Transaction] Handle acknowledgement in the transaction.

    https://github.com/apache/pulsar/pull/7856 (@[gaoran10](https://github.com/gaoran10))

- [Transaction] Support aborting transaction on partitions.

    https://github.com/apache/pulsar/pull/7953 (@[gaoran10](https://github.com/gaoran10))

- [Transaction] Optimize the logic for consuming transaction messages.

    https://github.com/apache/pulsar/pull/7833 (@[gaoran10](https://github.com/gaoran10))

- [Topic Policy] Support setting, getting, and removing `inactiveTopicPolicies` on the topic level.

    https://github.com/apache/pulsar/pull/7986 (@[315157973](https://github.com/315157973))

- [Topic Policy] Support offload policy on the topic level.

    https://github.com/apache/pulsar/pull/7883 (@[315157973](https://github.com/315157973))

- [Topic Policy] Support setting, getting, and removing `maxProducers` on the topic level.

    https://github.com/apache/pulsar/pull/7914 (@[zhanghaou](https://github.com/zhanghaou))

- [Topic Policy] Support compaction threshold on the topic level.

    https://github.com/apache/pulsar/pull/7881 (@[hangc0276](https://github.com/hangc0276))

### Notable Bug Fix

- [Broker] Fix NPE when acknowledging messages at the broker side.

    https://github.com/apache/pulsar/pull/7937 (@[Technoboy-](https://github.com/Technoboy-))

- [Broker] Stop dispatching messages when messages are skipped temporarily since the Key_Shared consumer is stuck on delivery.
    
    https://github.com/apache/pulsar/pull/7553 (@[equanz](https://github.com/equanz))

- [Metrics] Fix Pulsar metrics that provide wrong information.

    https://github.com/apache/pulsar/pull/7905 (@[315157973](https://github.com/315157973))

### Event / News
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020
 
     https://pulsar-summit.org/en/event/asia-2020

  - 09/09: "Apache Pulsar: Under the Hood for Java Developers" by Addison Higham in the Israeli Java Community (Java.IL)

    http://meetup.com/JavaIL/events/272501454/

### Blog / Article

- The role of Apache BookKeeper in Apache Pulsar - part 1 - Bartosz Konieczny

  -  https://www.waitingforcode.com/apache-pulsar/role-apache-bookkeeper-apache-pulsar-part-1/read

- 10 Reasons for Choosing Apache Pulsar over Apache Kafka

  - https://maximilianmichels.com/2020/apache-pulsar-vs-apache-kafka/

- Pulsar Summit Asia 2020 CFP is now open

  - http://pulsar.apache.org/blog/2020/08/25/pulsar-summit-asia-2020-cfp/
