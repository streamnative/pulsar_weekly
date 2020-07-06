---
title: "2020-06-26-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-06-20 ~ 2020-06-26"
date: 2020-06-20 ~ 2020-06-26
description: "This is the Pulsar community weekly update for 2020-06-20 ~ 2020-06-26, with updates on Pulsar 2.6.0 release, Pulsar Go client 0.1.1 release, Pulsar Manager 0.2.0 release, and so on."
id: "2020-06-26-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-06-20 ~ 2020-06-26

This is the Pulsar community weekly update for 2020-06-20 ~ 2020-06-26, with updates on Pulsar 2.6.0 release, Pulsar Go client 0.1.1 release, Pulsar Manager 0.2.0 release, and so on.

### Development

- [Release] Apache Pulsar 2.6.0 is released.
  
    https://lists.apache.org/thread.html/r3bbe7e31a0c7645c7dd77ce97141973c274c8e4dde787b471433c9f0%40%3Cdev.pulsar.apache.org%3E
    
    https://streamnative.io/blog/tech/2020-06-18-pulsar-260

- [Release] Apache Pulsar Go Client 0.1.1 is released.

    https://lists.apache.org/thread.html/r02a974daea1d26472ee1b9e9c4f5989633c1eb07886d6f17aff17fc7%40%3Cdev.pulsar.apache.org%3E

    https://github.com/apache/pulsar-client-go/releases/tag/v0.1.1

### Notable Feature

- [Helm] Remove helm chart since the helm chart is already moved to [pulsar-helm-chart](https://github.com/apache/pulsar-helm-chart).
  
    https://github.com/apache/pulsar/pull/7320

- [Function] Re-work Function MetaDataManager to make all metadata writes only by the leader.

    https://github.com/apache/pulsar/pull/7255

- [Function] Add statistics and Prometheus to Go Function instances for production readiness.

    https://github.com/apache/pulsar/pull/6105

- [Function] Add an endpoint to check whether function worker service is initialized.
  
    https://github.com/apache/pulsar/pull/7350

### Notable Bug Fix

- [Security] Fix the authorization regression in `isSupperUser`.

    https://github.com/apache/pulsar/pull/7241

- [Storage] Fix the issue of producers are stuck on creating ledger timeout.

    https://github.com/apache/pulsar/pull/7319

- [Functions] Fix race condition in which `exitFuture` in `FunctionAssignmentTailer` never gets completed even though the tailer thread has exited.
   
    https://github.com/apache/pulsar/pull/7351

### Ecosystem

- [Pulsar Manager] Apache Pulsar Manager 0.2.0 release is under discussion.
  
    https://lists.apache.org/thread.html/r4aef9dfedb4991a3ba7981d4065d717e436d8d3b2d2455cf6796cf87%40%3Cdev.pulsar.apache.org%3E

- [Pulsarctl] "Accept Pulsarctl as a part of Apache Pulsar project" is under discussion and in the vote. 

    https://lists.apache.org/thread.html/r8bbe89753c1162938086ad088f9267e1139f5d04108c872f3e34feec%40%3Cdev.pulsar.apache.org%3E

### Event / News

- [Pulsar Summit] The first-ever Pulsar Summit Virtual Conference 2020 was held on June 17 - 18. This two-day digital event featured more than 30 sessions from top Pulsar contributors and developers.

    All recordings and slides are available at [here](https://streamnative.io/resource#pulsar-summit). 
    
- [Meetup] Andreas Koestler gave a talk about "Scaling out WebSockets, Streams, Communicating FSMs and Apache Pulsar!" at Scala in the City Conference.

    https://www.signifytechnology.com/blog/2020/06/connecting-millions-of-users-by-andreas-koestler-at-scala-in-the-city-conference
    
- [TGIP] Weekly live stream about Pulsar and its ecosystem

    - 014: Pulsar Schema and Flink Integration - Sijie Guo

        - Recording: https://www.youtube.com/watch?v=Tc6vwyzzsh4&t=293s

### Blog / Article
        
- Event-driven Functions with Apache Pulsar & Project Flogo - Matt Ellis

    https://hackernoon.com/event-driven-functions-with-apache-pulsar-and-project-flogo-wag3y4u

- Creating an External Scaler for KEDA - Krishnaraj Varma

    https://medium.com/@krvarma/creating-an-external-scaler-for-keda-31b314b5c4a3
    