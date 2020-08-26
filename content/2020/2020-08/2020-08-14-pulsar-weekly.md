---
title: "2020-08-14-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-08-08 ~ 2020-08-14"
date: 2020-08-08 ~ 2020-08-14
description: "This is the Pulsar community weekly update for 2020-08-08 ~ 2020-08-14, with updates on Pulsar transaction, clients, brokers, security, Pulsar IO, and so on."
id: "2020-08-14-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-08-08 ~ 2020-08-14

This is the Pulsar community weekly update for 2020-08-08 ~ 2020-08-14, with updates on Pulsar transaction, clients, brokers, security, Pulsar IO, and so on.

### Development

- [Transaction] Support consuming transaction messages.
  
    https://github.com/apache/pulsar/pull/7781

- [Transaction] Support producing transaction messages to the Pulsar broker and executing the commit command.
  
    https://github.com/apache/pulsar/pull/7552

- [Topic Policy] Support setting retention on topic level.
  
    https://github.com/apache/pulsar/pull/7747

- [Topic policy] Support setting `MaxUnackMessagesPerSubscription` on topic level.
  
    https://github.com/apache/pulsar/pull/7802

- [Topic policy] Support the topic-level delayed delivery policy.
  
    https://github.com/apache/pulsar/pull/7784

- [Build] Upgrade Presto to version 332.
  
    https://github.com/apache/pulsar/pull/7194

- [Pulsar-IO hdfs2] Add configuration to create subdirectory from current time.
  
    https://github.com/apache/pulsar/pull/7771

- [Broker] Make ZooKeeper cache executor thread pool size configurable.

    https://github.com/apache/pulsar/pull/7794

- [Broker] Make orderedExecutor threads number configurable.

    https://github.com/apache/pulsar/pull/7765

### Notable Bug Fix

- [Security] Fix security vulnerabilities of Pulsar.
  
    https://github.com/apache/pulsar/pull/7801

- [Security] Use `allowTopicOperationAsync` to check whether the original role is a super user.

    https://github.com/apache/pulsar/pull/7788

- [Security] Differentiate authorization between source/sink/function operations.

    https://github.com/apache/pulsar/pull/7466

- [CPP client] Fix the issuer_url parsing failure in Oauth2 authentication.

    https://github.com/apache/pulsar/pull/7791

- [CPP client] Fix reference leak when creating the reader.
  
    https://github.com/apache/pulsar/pull/7793

- [Admin Client] Ensure to return Error 404 when deleting a partitioned topic from a non-existing namespace.

    https://github.com/apache/pulsar/pull/7777

- [Broker] Fix producer stucks on creating ledger timeout.

    https://github.com/apache/pulsar/pull/7319

### Event / News
  
- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Upcoming event]

  - 08/25: StreamNative Webinar - "Managing Real-Time Data Teams" by Jesse Anderson

    Registration link: https://us02web.zoom.us/webinar/register/6715970153506/WN_fEFcuXVFRWaZxa2pJtP3nQ

  - 09/09 "Apache Pulsar: Under the Hood for Java Developers" by Addison Higham in the Israeli Java Community (Java.IL)

    http://meetup.com/JavaIL/events/272501454/