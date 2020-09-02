---
title: "2020-08-28-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-08-22 ~ 2020-08-28"
date: 2020-08-22 ~ 2020-08-28
description: "This is the Pulsar community weekly update for 2020-08-22 ~ 2020-08-28, with updates on Pulsar clients, brokers, and so on."
id: "2020-08-28-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-08-22 ~ 2020-08-28

This is the Pulsar community weekly update for 2020-08-22 ~ 2020-08-28, with updates on Pulsar clients, brokers, and so on.

### Notable Feature

- [Broker] Add the hostname to consumer/producer properties in Pulsar Functions.

  https://github.com/apache/pulsar/pull/7897 (@[jerrypeng](https://github.com/jerrypeng))
  
- [Broker] Add the Java 8 date and time type to Pulsar primitive schemas.

  https://github.com/apache/pulsar/pull/7874 (@[jianyun8023](https://github.com/jianyun8023))

- [Broker] Add ability for `BatchPushSource` to notify errors asynchronously.

  https://github.com/apache/pulsar/pull/7865/files (@[jerrypeng](https://github.com/jerrypeng))
  
- [Broker] Support setting the message dispatch rate on the topic level.

  https://github.com/apache/pulsar/pull/7863 (@[hangc0276](https://github.com/hangc0276))

### Notable Bug Fix

- [CPP Client] Make `clear()` methods of `BatchAcknowledgementTracker` and `UnAckedMessageTrackerEnabled` thread-safe.

  https://github.com/apache/pulsar/pull/7862 (@[BewareMyPower](https://github.com/BewareMyPower))
  
- [Broker] Split message ranges by the ledger ID and store them in `individualDeletedMessages`.

  https://github.com/apache/pulsar/pull/7861 (@[massakam](https://github.com/massakam))

- [Broker] Fix deadlock which occurred when adding consumers.

  https://github.com/apache/pulsar/pull/7841 (@[massakam](https://github.com/massakam))
  
- [CPP Client] Throw std::exception types.

  https://github.com/apache/pulsar/pull/7798 (@[Bklyn](https://github.com/Bklyn))

### Event / News
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Event]

  - 08/25: StreamNative Webinar - "Managing Real-Time Data Teams" by Jesse Anderson

       - Video: https://www.youtube.com/watch?v=Owl_ncQbVwk
       - Slides：https://www.slideshare.net/JesseAnderson/managing-realtime-data-teams

  - 09/09: "Apache Pulsar: Under the Hood for Java Developers" by Addison Higham in the Israeli Java Community (Java.IL)

    http://meetup.com/JavaIL/events/272501454/

### Blog / Article

- Apache Pulsar 2.6.1

  - https://streamnative.io/blog/tech/2020-08-21-pulsar-261

- Apache Pulsar Celebrates 300th contributor

  - https://streamnative.io/blog/tech/2020-08-24-pulsar-300-contributors
