---
title: "2020-12-11-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-12-05 ~ 2020-12-11"
date: 2020-12-05 ~ 2020-12-11
description: "This is the Pulsar community weekly update for 2020-12-05 ~ 2020-12-11, with updates on Pulsar client, broker, Functions, and so on."
id: "2020-12-11-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-12-05 ~ 2020-12-11

This is the Pulsar community weekly update for 2020-12-05 ~ 2020-12-11, with updates on Pulsar client, broker, Functions, and so on.

### Pulsar Highlight

- [Broker] Export Prometheus metrics for messageTTL.

    https://github.com/apache/pulsar/pull/8871 

    by ([@315157973](https://github.com/315157973))

- [Function] Make the Schema information of the source topic available to downstream Sinks.

    https://github.com/apache/pulsar/pull/8854 

    by ([@eolivelli](https://github.com/eolivelli))

- [Function] Support fetching URLs for Go and Python functions.

    https://github.com/apache/pulsar/pull/8808 

    by ([@wolfstudy](https://github.com/wolfstudy))

- [Broker] Implement the packages management administration operations.

    https://github.com/apache/pulsar/pull/8816 
    
    by ([@zymap](https://github.com/zymap))

### Notable Feature

- [Broker] Export Prometheus metrics for messageTTL.

    https://github.com/apache/pulsar/pull/8871 ([@315157973](https://github.com/315157973))
    
- [Broker] Add REST APIs for package management service.

    https://github.com/apache/pulsar/pull/8858 ([@zymap](https://github.com/zymap))
    
- [Broker] Add the package management service into the Pulsar startup process.

    https://github.com/apache/pulsar/pull/8764 ([@zymap](https://github.com/zymap))

- [Broker] Change the `getWebServiceUrl` method into async.

    https://github.com/apache/pulsar/pull/8746 ([@reswqa](https://github.com/reswqa))
    
- [Broker] Support the package management client command.

    https://github.com/apache/pulsar/pull/8817 ([@zymap](https://github.com/zymap))
    
- [Broker] Implement the packages management administration operations.

    https://github.com/apache/pulsar/pull/8816 ([@zymap](https://github.com/zymap))
    
- [Function] Make Source topic Schema information available to downstream Sinks.

    https://github.com/apache/pulsar/pull/8854 ([@eolivelli](https://github.com/eolivelli))

- [Function][Function Worker] Splitting the authentication logic of function worker and client.

    https://github.com/apache/pulsar/pull/8824 ([@nodece](https://github.com/nodece))
    
- [Function] Support fetching URLs for Go and Python functions.

    https://github.com/apache/pulsar/pull/8808 ([@wolfstudy](https://github.com/wolfstudy))

- [Function] Add the command flag of `--retain-key-ordering` to Pulsar Functions.

    https://github.com/apache/pulsar/pull/8886 ([@wolfstudy](https://github.com/wolfstudy))

- [C++ Client] Add a setter for the reader's internal subscription name.

    https://github.com/apache/pulsar/pull/8823 ([@RobertIndie](https://github.com/RobertIndie))
    
- [Test] pulsar-perf supports more consumers per subscription.

    https://github.com/apache/pulsar/pull/8837 ([@Gjiangtao](https://github.com/Gjiangtao))
    
- [Java Client] Add a setter for the reader's subscription name.

    https://github.com/apache/pulsar/pull/8801 ([@315157973](https://github.com/315157973))

### Notable Bug Fix

- [C++ Client] Fix the race condition in `BlockingQueue`.

    https://github.com/apache/pulsar/pull/8765 ([@erobot](https://github.com/erobot))

- [Broker] Remove non-persistent subscriptions of topics from different threads to avoid deadlock when removing inactive subscriptions.

    https://github.com/apache/pulsar/pull/8820 ([@mkozioro](https://github.com/mkozioro))

- [Broker] Fix the performance issue caused by invalid logging configuration.

    https://github.com/apache/pulsar/pull/8908 ([@lhotari](https://github.com/lhotari))
    
- [Broker] Copy the list of subscriptions when checking for message expiration to avoid deadlocks.

    https://github.com/apache/pulsar/pull/8877 ([@massakam](https://github.com/massakam))
    
- [Broker] Fix the issue that an empty topic fails to get `lastMessageId` due to message retention.

    https://github.com/apache/pulsar/pull/8725 ([@eolivelli](https://github.com/eolivelli))
    
- [Broker] Ensure to updating the rack information dynamically.

    https://github.com/apache/pulsar/pull/8844 ([@k2la](https://github.com/k2la))
    
- [Schema] `GenericJsonReader` converts the null value to string "null".

    https://github.com/apache/pulsar/pull/8883 ([@eolivelli](https://github.com/eolivelli))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- Pulsar User Survey 2020

  - https://forms.office.com/Pages/ResponsePage.aspx?id=2zjkx2LkIkypCsNYsWmAs96ZDwmey39DhXAvi6EqbJpUNlZWQzRPMlVWNTc1WUcwUE5CWFMyUlI3QS4u

- Pulsar Summit Asia 2020

   - https://www.youtube.com/watch?v=4uB8i4zZXSw&list=PLqRma1oIkcWjHlRb-dzjwYdETkVlyCJOq
