---
title: "2020-09-25-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-09-19 ~ 2020-09-25"
date: 2020-09-19 ~ 2020-09-25
description: "This is the Pulsar community weekly update for 2020-09-19 ~ 2020-09-25, with updates on Pulsar client, broker, Pulsar SQL, Pulsar Functions, and so on."
id: "2020-09-25-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-09-19 ~ 2020-09-25

This is the Pulsar community weekly update for 2020-09-19 ~ 2020-09-25, with updates on Pulsar client, broker, Pulsar SQL, Pulsar Functions, and so on.

### Development

- [Broker] Use SNI for the TLS-enabled Pulsar Java broker client.

    https://github.com/apache/pulsar/pull/8117(@[racorn](https://github.com/racorn))

- [Pulsar SQL] Replace `com.ning.asynchttpclient` with `org.asynchttpclient` to enhance security.

    https://github.com/apache/pulsar/pull/8099(@[zymap](https://github.com/zymap))

- [Functions] Support specifying the secrets class in the localrunner builder.

    https://github.com/apache/pulsar/pull/8127(@[srkukarni](https://github.com/srkukarni))

- [Websocket] The WebSocket API supports unsubscribing from a topic.

    https://github.com/apache/pulsar/pull/8068(@[315157973](https://github.com/315157973))

- [Websocket] The WebSocket interface supports decoding URL for the topic name and subscription.

    https://github.com/apache/pulsar/pull/8072(@[315157973](https://github.com/315157973))

- [Broker] Support configuring the number of channels per bookie.

    https://github.com/apache/pulsar/pull/7910(@[rdhabalia](https://github.com/rdhabalia))

- [Functions] Support specifying the environment based on the secrets provider for source/sink/functions localrunner.

    https://github.com/apache/pulsar/pull/8098(@[srkukarni](https://github.com/srkukarni))

- [Client] Add a REST endpoint to trigger `backlogQuotaCheck`.

    https://github.com/apache/pulsar/pull/8045(@[315157973](https://github.com/315157973))

- [pulsar-client] Support non-durable subscription for pulsar-client commands.

    https://github.com/apache/pulsar/pull/8100(@[315157973](https://github.com/315157973))

- [Functions] Enable reporting functions worker JVM metrics through Prometheus.

    https://github.com/apache/pulsar/pull/8097(@[jerrypeng](https://github.com/jerrypeng))

- [Broker] Add replicated subscription check to `checkInactiveSubscriptions`.

    https://github.com/apache/pulsar/pull/8066(@[shustsud](https://github.com/shustsud))

- [Client] Support forcedly deleting all resources related to the namespace.

    https://github.com/apache/pulsar/pull/7993(@[murong00](https://github.com/murong00))

- [Topic Policy] Support setting, getting, and removing the subscription-based dispatch rate on the topic level.

    https://github.com/apache/pulsar/pull/8087(@[hangc0276](https://github.com/hangc0276))

- [Topic Policy] Support setting, getting, and removing the subscribe rate on the topic level.

    https://github.com/apache/pulsar/pull/7991(@[hangc0276](https://github.com/hangc0276))

- [Client] Support dynamically loading the Truststore certificate through the input stream.
	
    https://github.com/apache/pulsar/pull/7442(@[rdhabalia](https://github.com/rdhabalia))

- [Broker] Replace `IdentityHashMap` with `set -- Collections.newSetFromMap(new ConcurrentHashMap<>())` to hold the reference of producers/consumers.

    https://github.com/apache/pulsar/pull/8051(@[Technoboy-](https://github.com/Technoboy-))

### Notable Bug Fix

- [Functions] Fix Pulsar Functions threaded integration tests.

   https://github.com/apache/pulsar/pull/8118(@[jerrypeng](https://github.com/jerrypeng))

- [Client] Use the bytes of messages instead the number of messages for the producer to pend messages.

    https://github.com/apache/pulsar/pull/7957(@[Renkai](https://github.com/Renkai))

- [Client] Fix the issue that the client lookup hangs when the broker restarts.

    https://github.com/apache/pulsar/pull/8101(@[4onni](https://github.com/4onni))

- [Broker] Exclude the owner that does not belong to the current server.

    https://github.com/apache/pulsar/pull/8111(@[congbobo184](https://github.com/congbobo184))

- [Client] Avoid resolving the address for the SNI host while creating connection with SNI headers.

    https://github.com/apache/pulsar/pull/8062(@[rdhabalia](https://github.com/rdhabalia))

- [C++ Client] Add the Snappy library to Docker images for building C++ packages.

    https://github.com/apache/pulsar/pull/8086(@[massakam](https://github.com/massakam))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming Event]

  -  Pulsar Summit Asia 2020

     https://pulsar-summit.org/en/event/asia-2020

  - Low-Latency Stream Processing with Jet

    https://us02web.zoom.us/webinar/register/3216003857537/WN_821OFj6ITN23Y8uf8KgEag
    
  - [Pulsar Training] Developing Pulsar Applications with Jesse Anderson

    https://www.eventbrite.com/e/developing-pulsar-applications-online-training-tickets-122334542911

### Blog / Article

- Evaluating Apache Pulsar - Luke Stephenson

  - https://medium.com/zendesk-engineering/evaluating-apache-pulsar-92e6ed3fc792

- Announcing MQTT-on-Pulsar: Bringing Native MQTT Protocol Support to Apache Pulsar

  - https://streamnative.io/blog/tech/2020-09-28-announcing-mqtt-on-pulsar