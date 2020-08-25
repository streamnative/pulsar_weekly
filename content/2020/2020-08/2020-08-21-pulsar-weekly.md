---
title: "2020-08-21-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-08-15 ~ 2020-08-21"
date: 2020-08-15 ~ 2020-08-21
description: "This is the Pulsar community weekly update for 2020-08-15 ~ 2020-08-21, with updates on Pulsar clients, brokers, and so on."
id: "2020-08-21-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-08-15 ~ 2020-08-21

This is the Pulsar community weekly update for 2020-08-15 ~ 2020-08-21, with updates on Pulsar clients, brokers, and so on.

### Notable Feature

- [Broker] Support `MaxUnackedMessagesOnConsumer` on topic level.

    https://github.com/apache/pulsar/pull/7818 (@[315157973](https://github.com/315157973))
    
- [Broker] Support persistence policies on topic level.

    https://github.com/apache/pulsar/pull/7817 (@[zhanghaou](https://github.com/zhanghaou))
    
- [Broker] Support deduplication on topic level.

    https://github.com/apache/pulsar/pull/7821 (@[315157973](https://github.com/315157973))

- [Java Client] Support acknowledging a list of messages.

    https://github.com/apache/pulsar/pull/7688 (@[315157973](https://github.com/315157973))
    
- [Python CLient] Add oauth2 client wrapper for the Python client.

    https://github.com/apache/pulsar/pull/7813 (@[jiazhai](https://github.com/jiazhai))
    
- [Java Client] Expose `autoPartitionsUpdateInterval` for the producer and consumer.

    https://github.com/apache/pulsar/pull/7840 (@[RobertIndie](https://github.com/RobertIndie))
    
### Notable Bug Fix

- [Java Client] Avoid subscribing the same topic again.

    https://github.com/apache/pulsar/pull/7823 (@[BewareMyPower](https://github.com/BewareMyPower))
    
- [Broker] Redirect to get messages by ID request when a broker does not serve for the topic.

    https://github.com/apache/pulsar/pull/7786 (@[rudy2steiner](https://github.com/rudy2steiner))

- [Java Client] Fix the pending batchIndexAcks, bitSet, and batchSize in PersistentAcknowledgmentsGroupingTracker.

    https://github.com/apache/pulsar/pull/7828 (@[gaoran10](https://github.com/gaoran10))

- [CPP Client] Fix race condition caused by seeking or closing the consumer.

    https://github.com/apache/pulsar/pull/7819 (@[jiazhai](https://github.com/jiazhai))

### Event / News
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming event]

  - 08/25: StreamNative Webinar - "Managing Real-Time Data Teams" by Jesse Anderson

    Registration link: https://us02web.zoom.us/webinar/register/6715970153506/WN_fEFcuXVFRWaZxa2pJtP3nQ

  - 09/09: "Apache Pulsar: Under the Hood for Java Developers" by Addison Higham in the Israeli Java Community (Java.IL)

    http://meetup.com/JavaIL/events/272501454/

### Blog / Article

- Announcing StreamNative Cloud - Apache Pulsar as a Service (Eron Wright & Sijie Guo)

  - https://streamnative.io/blog/tech/2020-08-18-announcing-streamnative-cloud
