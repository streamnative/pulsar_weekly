---
title: "2021-03-15-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-03-08 ~ 2021-03-14"
date: 2021-03-08 ~ 2021-03-14
description: "This is the Pulsar community weekly update for 2021-03-08 ~ 2021-03-14, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-03-15-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-03-08 ~ 2021-03-14

This is the Pulsar community weekly update for 2021-03-08 ~ 2021-03-14, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

The WebSocket client supports the token authentication.

by ([@gaoran10](https://github.com/gaoran10))

### Development

- [C++ Client] Implement memory limit in C++ producer.

    https://github.com/apache/pulsar/pull/9676 ([@merlimat](https://github.com/merlimat))

- [Transactions] Support checking the transaction state.

    https://github.com/apache/pulsar/pull/9776 ([@congbobo184](https://github.com/congbobo184))

- [Transactions] Implement the transaction buffer snapshot. 

    https://github.com/apache/pulsar/pull/9490 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Support getting applied `PersistencePolicies`.

    https://github.com/apache/pulsar/pull/9831 ([@315157973](https://github.com/315157973))

- [Broker] Support getting applied `clusterSubscribeRate`.

    https://github.com/apache/pulsar/pull/9832 ([@315157973](https://github.com/315157973))

- [Broker] Support getting applied `dispatchRate`.

    https://github.com/apache/pulsar/pull/9824 ([@315157973](https://github.com/315157973))

- [pulsar-admin] Add the command to get service URL of the leader broker.

    https://github.com/apache/pulsar/pull/9799 ([@linlinnn](https://github.com/linlinnn))

- [Pulsar Client] Support printing `GenericRecord` contents.

    https://github.com/apache/pulsar/pull/9785 ([@eolivelli](https://github.com/eolivelli))

- [WebSocket Client] Make the browser client support the token authentication.

    https://github.com/apache/pulsar/pull/9886 ([@gaoran10](https://github.com/gaoran10))

### Notable Bug Fix

- [Broker] Continue to gracefully shut down the broker service even the web service fails to be closed.

    https://github.com/apache/pulsar/pull/9835 ([@massakam](https://github.com/massakam))

- [Topic] Automatically create partitions even when auto-creation is disabled.

    https://github.com/apache/pulsar/pull/9786 ([@mlyahmed](https://github.com/mlyahmed))

- [Consumer] Delete disconnected consumers to allow auto-discovery.

    https://github.com/apache/pulsar/pull/9660 ([@mlyahmed](https://github.com/mlyahmed))

- [Broker] Log stacktraces of threads that failed to terminate on shutdown within timeout in ExecutorProvider.

    https://github.com/apache/pulsar/pull/9840 ([@jerrypeng](https://github.com/jerrypeng))

- [pulsar-perf] Fix the pulsar-perf CLI tool to keep compatibility with previous versions.

    https://github.com/apache/pulsar/pull/9838 ([@murong00](https://github.com/murong00))

- [Broker] Support disabling the tenants/namespaces force deletion in the `broker.conf` file.

    https://github.com/apache/pulsar/pull/9819 ([@murong00](https://github.com/murong00))

- [Broker] Allow the broker to discover and unblock stuck subscriptions.

    https://github.com/apache/pulsar/pull/9789 ([@rdhabalia](https://github.com/rdhabalia))

- [Schema] Expose the native record for the struct schema.

    https://github.com/apache/pulsar/pull/9614 ([@eolivelli](https://github.com/eolivelli))

- [Client] Ensure the single-topic consumer can be closed.

    https://github.com/apache/pulsar/pull/9849 ([@HugeSkull](https://github.com/HugeSkull))

- [Schema] Fix the issue that schema is not added when the consumer subscribes an empty topic without schema.

    https://github.com/apache/pulsar/pull/9853 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Client] Fix the issue that the batch size is not set when being deserialized from the byte array.

    https://github.com/apache/pulsar/pull/9855 ([@zymap](https://github.com/zymap)

- [Schema] Add the schema type validation.

    https://github.com/apache/pulsar/pull/9797 ([@limingnihao](https://github.com/limingnihao))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - TGIP 20: March Updates on Apache Pulsar
     
     - https://www.youtube.com/watch?v=fgFTzmdTVQE

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

### Blog / Article

- TIntroducing the Apache Pulsar Hackathon 2021

    - https://streamnative.io/en/blog/community/2021-03-11-introducing-the-apache-pulsar-hackathon-2021

- How To Get Started With Apache Pulsar On Docker

    - https://www.lionbloggertech.com/apache-pulsar-on-docker/?utm_source=ReviveOldPost&utm_medium=social&utm_campaign=ReviveOldPost 
