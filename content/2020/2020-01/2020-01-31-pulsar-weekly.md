---
title: "2020-01-31-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-01-18 ~ 2020-01-31"
date: 2020-01-18 ~ 2020-01-31
description: "This is the Pulsar community weekly update for 2020-01-18 ~ 2020-01-31, with updates on Pulsar CI, release process, community growth, and activities"
---

## [Pulsar Community Weekly Update] 2020-01-18 ~ 2020-01-31

This is the Pulsar community weekly update for 2020-01-18 ~ 2020-01-31, with updates on Pulsar CI, release process, community growth, and activities.

### Development

- [CI] Pulsar has migrated to use GitHub Actions for CI. GitHub Actions provide more resources for running CI jobs. Although there are still flaky tests. Multiple committers are working on improving those tests.


- [Project] DotPulsar was accepted as a sub-project of Apache Pulsar.

    https://lists.apache.org/thread.html/rc7bbb49a94e121b0db2e48ce0f30986d507c2589fb45d31dde736878%40%3Cdev.pulsar.apache.org%3E
    
- [Release] The community has voted to use `milestone` for tracking major releases and `label` for tracking minor releases.

    https://lists.apache.org/thread.html/r96e253dd36a90438247c904529a26feee2f3d4562895ef0489665de5%40%3Cdev.pulsar.apache.org%3E

### Notable Feature

- [Broker] Allow enabling / disabling delayed delivery for messages on namespace (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/5915

### Notable Bug Fix

- [Connector] Make type name of Elasticsearch sink connector configurable (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6028
    
- [Client] Fix zeroQueueConsumer using listener (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6106
    
- [Websocket] Websocket doesn't set the correct cluster data (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6102

### Event / News

- [Podcast] "Taking messaging and data ingestion systems to the next level" - Sijie Guo from StreamNative talked about "How Apache Pulsar is able to handle both queuing and streaming, and both online and offline applications." on Data Exchange Podcast.

    https://thedataexchange.media/taking-messaging-and-data-ingestion-systems-to-the-next-level
    
- [Conference] Data Day Texas was held on January 25, 2020 in Austin. Three presentations of Pulsar were presented there.

    - "Building a streaming data warehouse using Flink and Pulsar" - presented by Sijie Guo from StreamNative.
    
        https://datadaytexas.com/2020/sessions#guo
        
    - "AI / ML model serving using Apache Pulsar Functions" - presented by Karthik Ramasamy from Splunk.
    
        https://datadaytexas.com/2020/sessions#ramasamy1
        
    - "Using interactive querying of streaming data for anomaly detection" - presented by Karthik Ramasamy from Splunk.

        https://datadaytexas.com/2020/sessions#ramasamy1

- [Survey] The Pulsar User Survey will be closed on February 9. Your feedback is highly appreciated.

    https://forms.office.com/Pages/ResponsePage.aspx?id=DQSIkWdsW0yxEjajBLZtrQAAAAAAAAAAAAZAAOjIXw9UMUNLRUdJMVJBS1RRNjVNNjMzR0JPTFpGWi4u

- [Conference] Call for Presentations for the first Pulsar Summit is extended to February 14. The conference will be held on April 28th, 2020 at San Francisco. The pre-registration is also open.

    - Call for presentation: https://pulsar-summit.org/call-for-presentations/
    
    - Pre-registration: https://pulsar-summit.org/pre-registration/
    
- [Growth] Pulsar community keeps on growing.

    - The number of stars for the Pulsar GitHub Repository has exceeded 5000.

        https://github.com/apache/pulsar
     
    - The number of Pulsar Slack users has exceeded 1500.

        https://twitter.com/karthikz/status/1223405490454986753

