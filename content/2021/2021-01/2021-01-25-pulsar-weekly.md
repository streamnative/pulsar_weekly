---
title: "2021-01-25-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-01-18 ~ 2021-01-24"
date: 2021-01-18 ~ 2021-01-24
description: "This is the Pulsar community weekly update for 2021-01-18 ~ 2021-01-24, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-01-25-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-01-18 ~ 2021-01-24

This is the Pulsar community weekly update for 2021-01-18 ~ 2021-01-24, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Pulsar Highlight

Implement `CoordinationService` abstraction on the top of `MetadataStore` to realize the following operations:

- Lock management
- Leader election
- Unique number generator

By ([@merlimat](https://github.com/merlimat))

### Notable Feature

- [Topic Policy] Support getting the applied policy for `InactiveTopic`.

    https://github.com/apache/pulsar/pull/9230 ([@315157973](https://github.com/315157973))

- [Interceptor] Skip the interceptor for `MediaType.MULTIPART_FORM_DATA`.

    https://github.com/apache/pulsar/pull/9217 ([@codelipenghui](https://github.com/codelipenghui))

- [Transactions] Implement the transaction buffer stable position and `lowWaterMark`.

    https://github.com/apache/pulsar/pull/9195 ([@congbobo184](https://github.com/congbobo184))

- [Plugin] Use the default ASF configuration to create the Source tarball.

    https://github.com/apache/pulsar/pull/9184 ([@eolivelli](https://github.com/eolivelli))

- [Authentication] Add the authentication action for the package management service.

    https://github.com/apache/pulsar/pull/8893 ([@zymap](https://github.com/zymap))

### Notable Bug Fix

- [Dependency] Remove Spring Plugins repository.

    https://github.com/apache/pulsar/pull/9280 ([@eolivelli](https://github.com/eolivelli))

- [Dependency] Remove the hbase-server dependency.

    https://github.com/apache/pulsar/pull/9278 ([@Renkai](https://github.com/Renkai))

- [C++] Fix the issue that `ServerError` is not converted to string in the log.

    https://github.com/apache/pulsar/pull/9277 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Topic Policy] Fix the Flaky unit test.

    https://github.com/apache/pulsar/pull/9262 ([@315157973](https://github.com/315157973))

- [Functions] Fix the issue that the Function worker does not use the `isSuperUser` method to check the status of the super user. 

    https://github.com/apache/pulsar/pull/9259 ([@zymap](https://github.com/zymap))

- [Broker] Fix the race condition on producer/consumer maps in `ServerCnx`.

    https://github.com/apache/pulsar/pull/9256 ([@ivankelly](https://github.com/ivankelly))
    
- [Broker] Fix the issue that the interceptor is disabled in `ResponseHandlerFilter.java`.

    https://github.com/apache/pulsar/pull/9252 ([@codelipenghui](https://github.com/codelipenghui))
    
- [Interceptor] Fix the issue that the interceptor does not handle boundary for multipart/form-data.

    https://github.com/apache/pulsar/pull/9247 ([@codelipenghui](https://github.com/codelipenghui))
    
- [Test] Clean up the Flaky test `BatchSourceExecutorTest`.

    https://github.com/apache/pulsar/pull/9243 ([@eolivelli](https://github.com/eolivelli))
    
- [Log] Provide the debug log for `OpAddEntry`.

    https://github.com/apache/pulsar/pull/9239 ([@Shoothzj](https://github.com/Shoothzj))

- [Broker] Handle web application exception to the redirect request.

    https://github.com/apache/pulsar/pull/9228 ([@sijie](https://github.com/sijie))

- [Flaky test] Fix unit tests that occasionally fail.

    https://github.com/apache/pulsar/pull/9226 ([@315157973](https://github.com/315157973))

- [Broker] Fix incorrect tips for errors of creating topics when the namespace does not exist.

    https://github.com/apache/pulsar/pull/9223 ([@aloyszhang](https://github.com/aloyszhang))

- [Broker] Fix mis-use of local/global ZooKeepers and provide different ZooKeepers for global/local in `MockedPulsarServiceBaseTest`.

    https://github.com/apache/pulsar/pull/9222 ([@aloyszhang](https://github.com/aloyszhang))

- [Broker] Fix the issue that `maxConsumersPerTopic` cannot be disabled at the namespace level.

    https://github.com/apache/pulsar/pull/9214 ([@315157973](https://github.com/315157973))

- [Compaction] Fix the issue with topic compaction when the compaction ledger is empty.

    https://github.com/apache/pulsar/pull/9206 ([@jerrypeng](https://github.com/jerrypeng))

- [Dead Letter Queue] Fix the issue with incorrect condition checj when creating producers for the Dead Letter Queue (DLQ).

    https://github.com/apache/pulsar/pull/9166 ([@MarvinCai](https://github.com/MarvinCai))

- [Build] Fix the issue with building the C++ client library on Mac OS if a different OpenSSL is used.

    https://github.com/apache/pulsar/pull/9165 ([@phijohns-tibco](https://github.com/phijohns-tibco))

### Event / News

- [Webinar] Watch Your Streams: Implementing OpenTelemetry with Apache Pulsar

    - https://us02web.zoom.us/webinar/register/3216003857537/WN_IyokJqHFRjicIuYT3ui4Ew

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- [Learning] Apache Pulsar: The Next Generation Messaging and Queuing System -- Karthik Ramasamy

    - https://www.youtube.com/watch?v=30QKArypisg

### Blog / Article

- StreamNative Launches Pulsar-as-a-Service on AWS

    - https://streamnative.io/en/blog/release/2021-01-21-streamnative-cloud-aws