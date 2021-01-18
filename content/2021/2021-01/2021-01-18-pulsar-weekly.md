---
title: "2021-01-18-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-01-11 ~ 2021-01-17"
date: 2021-01-11 ~ 2021-01-17
description: "This is the Pulsar community weekly update for 2021-01-11 ~ 2021-01-17, with updates on Pulsar client, broker, Functions, and so on."
id: "2021-01-18-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-01-11 ~ 2021-01-17

This is the Pulsar community weekly update for 2021-01-11 ~ 2021-01-17, with updates on Pulsar client, broker, Functions, and so on.

### Pulsar Highlight

Pulsar supports the dispatch rate policy for the replicator at the topic level.

By [@315157973](https://github.com/315157973)

### Notable Feature

- [Functions Worker] Support initializing the distributed log namespace metadata through `bin/pulsar`.

    https://github.com/apache/pulsar/pull/8781 ([@nodece](https://github.com/nodece))

- [Pulsar-broker-common] Move the additional Servlet module to the Pulsar broker common module.

    https://github.com/apache/pulsar/pull/9164 ([@tuteng](https://github.com/tuteng))

- [Bookie] Upgrade BookKeeper to version 4.12.1 to allow Pulsar to use the ID instead of the network address of the Bookie.

    https://github.com/apache/pulsar/pull/9019 ([@eolivelli](https://github.com/eolivelli))

- [Topic Policy] Support the dispatch rate policy for the replicator at the topic level.

    https://github.com/apache/pulsar/pull/9175 ([@315157973](https://github.com/315157973))

### Notable Bug Fix

- [C++] Fix the issue that `UnAckedMessageTracker` handles batch messages incorrectly.

    https://github.com/apache/pulsar/pull/9170 ([@saosir](https://github.com/saosir))

- [Client] Fix the issue that an user-unfriendly error message is sent when creating a sink without setting a name.

    https://github.com/apache/pulsar/pull/9131 ([@eolivelli](https://github.com/eolivelli))

- [Client] Fix the issue about the size of incoming messages.

    https://github.com/apache/pulsar/pull/9182 ([@codelipenghui](https://github.com/codelipenghui))

- Fix memory leak caused by the release of ByteBuf.

    https://github.com/apache/pulsar/pull/9194 ([@aloyszhang](https://github.com/aloyszhang))

- [Admin] Fix the issue that the URI resolution does not support multiple addresses.

    https://github.com/apache/pulsar/pull/9191 ([@315157973](https://github.com/315157973))

- [Admin] Fix a potential HTTP-get hangs in the Pulsar Admin since the callback might never be called.

    https://github.com/apache/pulsar/pull/9203 ([@codelipenghui](https://github.com/codelipenghui))

- [Admin] Fix the issue that the configuration of the maximum number of topics for a namespace does not work.

    https://github.com/apache/pulsar/pull/9193 ([@aloyszhang](https://github.com/aloyszhang))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Webinar] Watch Your Streams: Implementing OpenTelemetry with Apache Pulsar

    - https://us02web.zoom.us/webinar/register/3216003857537/WN_IyokJqHFRjicIuYT3ui4Ew

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq

### Blog / Article

- Taking a Deep-Dive into Apache Pulsar Architecture for Performance Tuning

    - https://streamnative.io/en/blog/tech/2021-01-14-pulsar-architecture-performance-tuning

- How Apache Pulsar is Helping Iterable Scale its Customer Engagement Platform

    - https://streamnative.io/en/success-stories/iterable
