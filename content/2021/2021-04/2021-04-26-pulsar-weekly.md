---
title: "2021-04-26-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-04-19 ~ 2021-04-25"
date: 2021-04-19 ~ 2021-04-25
description: "This is the Pulsar community weekly update for 2021-04-19 ~ 2021-04-25, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-04-26-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-04-19 ~ 2021-04-25

This is the Pulsar community weekly update for 2021-04-19 ~ 2021-04-25, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- Add some basic supports for testing de-duplication feature.

    by ([@klwilson227](https://github.com/klwilson227))

- Add `--topic-domain=persistent` and `--topic-domain=non-persistent` options to the pulsar-admin commands to get persistent topics and non-persistent topics.

    by ([@codelipenghui](https://github.com/codelipenghui))

- Upgrade Vert.x version to 3.9.7 to resolve vulnerability caused by version 3.5.3.

    by ([@lhotari](https://github.com/lhotari))

- Add basic configuration for the `org.owasp:dependency-check-maven` Maven plugin and make it operational in the Apache Pulsar project.

    by ([@lhotari](https://github.com/lhotari))

### Development

- [PIP-82] [Broker] Add support for distributed resource quota enforcement at the tenant, namespace or topic level.

    https://github.com/apache/pulsar/pull/10218 ([@ravi-vaidyanathan](https://github.com/ravi-vaidyanathan))

### Notable Bug Fix

- [pulsar-client] Fix inconsistent `equals` and `hashCode` methods for `MessageIds`.

    https://github.com/apache/pulsar/pull/9440 ([@gmethvin](https://github.com/gmethvin))

- [Broker] Fix the Log4j 2 logging issue occurred in the shutdown process of the broker.

    https://github.com/apache/pulsar/pull/10304 ([@lhotari](https://github.com/lhotari))

- [Transaction] Fix the transaction buffer operation failure.
    
    https://github.com/apache/pulsar/pull/10322 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Fix the transaction client timeout issue.
    
    https://github.com/apache/pulsar/pull/10323 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Fix the transaction client reconnection issue.
    
    https://github.com/apache/pulsar/pull/10327 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Fix the issue that `MLTransactionLog` generates the illegal `managedLedger` name.
    
    https://github.com/apache/pulsar/pull/10334 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Fix the issue that the transaction timeout tracker is expired.
    
    https://github.com/apache/pulsar/pull/10366 ([@congbobo184](https://github.com/congbobo184))


### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - 04/24: https://www.youtube.com/watch?v=JzExXJYiGvY&t=26s

- Apache Pulsar Hackathon

    Sign-up: https://www.eventbrite.com/e/apache-pulsar-hackathon-2021-tickets-143906003731

- Pulsar Virtual Summit North America 2021

    Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

### Blog / Article

- Flink SQL on StreamNative Cloud

    - https://streamnative.io/en/blog/release/2021-04-20-flink-sql-on-streamnative-cloud