---
title: "2019-12-06-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-11-30 ~ 2019-12-06"
date: 2019-11-30 ~ 2019-12-06
description: "This is the Pulsar community weekly update for 2019-11-30 ~ 2019-12-06, with updates on broker supports dispatch throttling relative to publish-rate, pulsar-manager supports user login, and the progress about Pulsar releases."
id: "2019-12-06-pulsar-weekly"
---

## [Puslar Community Weekly Update] 2019-11-30 ~ 2019-12-06

This is the Pulsar community weekly update for 2019-11-30 ~ 2019-12-06, with updates on broker supports dispatch throttling relative to publish-rate, pulsar-manager supports user login, and the progress about Pulsar releases. 

### Development

* Apache Pulsar 2.4.2 is released.

    https://lists.apache.org/thread.html/9a13692681c15396b295c1ced70714d2b926e4851ad923e77b1c9ce0%40%3Cdev.pulsar.apache.org%3E
    
    http://pulsar.apache.org/release-notes/#242-mdash-2019-12-04-a-id242a
    
* Pulsar 2.5.0 release is started.

    https://lists.apache.org/thread.html/41a6cf6d60bf593059e572fbf7a09d229c80fee1f532bfd375a165af%40%3Cdev.pulsar.apache.org%3E
    
* [PIP-52] Add support of dispatch throttling relative to publish-rate.

    https://github.com/apache/pulsar/pull/5797
    
    https://github.com/apache/pulsar/wiki/PIP-52%3A-Message-dispatch-throttling-relative-to-publish-rate
    
* [Pulsar Manager] The development of adding authentication and authorization support in Pulsar Manager continues. The pull request to support user login was merged.

    https://github.com/apache/pulsar-manager/pull/222

* Pulsar PMC has invited Yu Liu to become a Pulsar committer.

    https://lists.apache.org/thread.html/7269164410b0cffbfa563a8aa65c8e6de458db7019036d37424fba7e%40%3Cdev.pulsar.apache.org%3E

### Notable Feature

- [pulsar-client-python] Expose redelivery count of message in Python client.

    https://github.com/apache/pulsar/pull/5812

### Notable Bug Fix

- [broker] Create load balance znode of broker when znode missed.

    https://github.com/apache/pulsar/pull/5784

- [pulsar-perf] Fix ArrayIndexOutOfBoundsException in PerformanceProducer.

    https://github.com/apache/pulsar/pull/5786

- [pulsar-function-go] Fix a memory leak of pulsar-function-go library regarding time.NewTimer().

    https://github.com/apache/pulsar/pull/5627

### Ecosystem

* [FLINK-15089][connectors] Puslar catalog.

    https://github.com/apache/flink/pull/10455

### Event/News

* TIBCO adds support for Pulsar to messaging solution.

    https://www.tibco.com/press-releases/2019/tibco-adds-support-apache-pulsar-messaging-solution
    
    
* GitHub Meetup was held on Dec 4 in Beijing. Xiaolong Ran from StreamNative gave a talk about Go in Pulsar.

    https://www.slideshare.net/streamnative/apache-pulsar-and-githubxiaolong

### Blog/Article

* How to query Pulsar Streams using Flink (by Sijie Guo & Markos Sfikas)

    https://flink.apache.org/news/2019/11/25/query-pulsar-streams-using-apache-flink.html
    
* #Tech in 5 — Apache Pulsar: An Introductory Technical Assessment of Apache Pulsar and an Example of How to Make it Work for You (by Kieran Healey)

    https://medium.com/hashmapinc/tech-in-5-apache-pulsar-166330e6aceb