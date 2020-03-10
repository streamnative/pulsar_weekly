---
title: "2019-12-20-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-12-07 ~ 2019-12-20"
date: 2019-12-07 ~ 2019-12-20
description: "This is the Pulsar community weekly update for 2019-12-07 ~ 2019-12-20, with updates on DotPulsar, key windowed function, Pulsar Native Go client, batch authorization of partitioned topic, API document, and so on."
id: "2019-12-20-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2019-12-07 ~ 2019-12-20

This is the Pulsar community weekly update for 2019-12-07 ~ 2019-12-20, with updates on DotPulsar, key windowed function, Pulsar Native Go client, batch authorization of partitioned topic, API document, and so on.

### Development

- [PIP-53] Daniel Blankensteiner from Danske Commodities started the email thread of contributing DotPulsar (a Pulsar client library for .NET) to Apache Pulsar.

    https://lists.apache.org/thread.html/8ebe35027d818e595eec322da26a3f392324ec3d86c4c1b12b1ff498%40%3Cdev.pulsar.apache.org%3E
    
    https://github.com/danske-commodities/dotpulsar
    
- [Documentation] Guangning E has backfilled the API documentation for old releases. Now Pulsar has provided API documentations for each release.
         
    https://lists.apache.org/thread.html/83b33b81229a09fecf4a643c7e6704d75ab86f990ce2d676cf7f0ddd%40%3Cdev.pulsar.apache.org%3E

- [Native Go Client] Xiaolong Ran has initiated a discussion of creating the first official release for Pulsar Native Go client.

    https://lists.apache.org/thread.html/519d840d9e4843651ab8dc15515f25e8c5bf5212e79f2ad63f6d2cec%40%3Cdev.pulsar.apache.org%3E

- [Pulsar Function] A new proposal is raised for introducing key windowed function in Pulsar Functions.

    https://lists.apache.org/thread.html/5228bdddafb49badb2f25dbf4ab40e134d3c346933da2fcb0a6db36a%40%3Cdev.pulsar.apache.org%3E

- [Release] The first release candidate of Pulsar 2.5.0 release was cancelled for fixing bugs identified during voting.

    https://lists.apache.org/thread.html/7a050d26e327d09803de368ce109c7d61177131551bc5a114204a61b%40%3Cdev.pulsar.apache.org%3E


### Notable Feature

- [Security] Support batch authorization of partitioned topic (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/5767
    
- [Broker] Pulsar broker supports advertising IPV6 address (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5713

### Notable Bug Fix

- [Java][Client] Ensure that the same message ID is not added to UnAckedMessageTracker multiple times (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5823
    
- [Tiered Storage] Fix "s3 offloading generates huge zk txn logs in some conditions" (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5834

- [CLI] Make PulsarClusterMetadataSetup idempotent (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5879
    
### Event / News

- [Milestone] Pulsar has attracted its 200th contributor! It is an important milestone for our community growth.

    https://streamnative.io/blog/tech/2019-12-20-pulsar-milestone-celebration-200-contributors/

- [Conference] Pulsar Summit San Francisco 2020 Call for Presentation is open.

    https://pulsar.apache.org/blog/2019/12/18/Pulsar-summit-cfp/

- [Conference] Paris Open Source Summit 2019 was held on Dec 10 - 11 in France. Bruno Bonnin talked about "Stream Processing with Apache Pulsar" on this conference.

    https://speakerdeck.com/bbonnin/stream-processing-avec-apache-pulsar-b3106b65-5334-4d43-8934-a13884a6f5af

- [Meetup] GDG DevFest 2019 happened on Dec 8 in Beijing. Xiaolong Ran from StreamNative shared "Serverless Event Streaming with Pulsar Functions" on this meetup.

    https://www.slideshare.net/streamnative/google-devfest-about-pulsar-by-xiaolong

- [Conference] China Technical Communication Forum 2019 was held on Dec 7 in Beijing. Yu Liu from StreamNative gave a talk about the Pulsar doc development process, how the Docs Like Code solution improves the development efficiency and quality of Pulsar docs and recent updates in the Pulsar community.

    https://www.slideshare.net/streamnative/code-the-docsyu-liu

### Blog / Article

- The fourth chapter — Pulsar IO Connectors — is available in **Pulsar in Action** (by David Kjerrumgaard)

    https://www.manning.com/books/pulsar-in-action

- Apache Pulsar adapter for SAP PO (by Peter Ha)

    https://blogs.sap.com/2019/12/16/apache-pulsar-adapter-for-sap-po/?utm_source=dlvr.it&utm_medium=twitter

    