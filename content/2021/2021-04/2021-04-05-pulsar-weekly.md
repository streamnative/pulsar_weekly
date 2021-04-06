---
title: "2021-04-05-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-03-29 ~ 2021-04-04"
date: 2021-03-29 ~ 2021-04-04
description: "This is the Pulsar community weekly update for 2021-03-29 ~ 2021-04-04, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-04-05-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-03-29 ~ 2021-04-04

This is the Pulsar community weekly update for 2021-03-29 ~ 2021-04-04, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

Introduce the Pulsar Interface Taxonomy to guide developers and users to use Pulsar APIs.

by ([@sijie](https://github.com/sijie))

### Development

- [Transactions] Implement transaction pending-ack server patch.

    https://github.com/apache/pulsar/pull/8426 ([@congbobo184](https://github.com/congbobo184))

- [Transactions] Register the transaction metadata before sending or acknowledging messages.
    
    https://github.com/apache/pulsar/pull/8493 ([@gaoran10](https://github.com/gaoran10))

- [Transactions] Expose the transaction interface.
    
    https://github.com/apache/pulsar/pull/8505 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Expose consumer names after the `mark-delete-position` for the Key_Shared subscription.
    
    https://github.com/apache/pulsar/pull/8545 ([@codelipenghui](https://github.com/codelipenghui))

- [Transaction] Ensure that the transaction metadata handlers are connected.
    
    https://github.com/apache/pulsar/pull/8563 ([@gaoran10](https://github.com/gaoran10))

- [Bookie] Add the bookie client quarantine ratio configuration for bookie client 4.11.1.
    
    https://github.com/apache/pulsar/pull/8546 ([@hangc0276](https://github.com/hangc0276))

- [Broker] Improve the function state workflow with timeouts.
    
    https://github.com/apache/pulsar/pull/8528 ([@jerrypeng](https://github.com/jerrypeng)) 

### Notable Feature

- [Broker] Support taking de-duplication snapshots based on time.
    
    https://github.com/apache/pulsar/pull/8474 ([@315157973](https://github.com/315157973))

- [Broker] Support the namespace-level duplication snapshot.
    
    https://github.com/apache/pulsar/pull/8506 ([@315157973](https://github.com/315157973))

- [Broker] Introduce the Pulsar Interface Taxonomy to guide developers and users to use Pulsar APIs.
    
    https://github.com/apache/pulsar/pull/8530 ([@sijie](https://github.com/sijie))

### Notable Bug Fix

- [Broker] Fix the issue that is caused by cleaning inactive partitioned topics.
    
    https://github.com/apache/pulsar/pull/8442 ([@315157973](https://github.com/315157973))

- [C++] Catch the exception thrown by the remote endpoint.
    
    https://github.com/apache/pulsar/pull/8486 ([@BewareMyPower](https://github.com/BewareMyPower))

- [Transactions] Fix the `TransactionBufferHandlerImpl` thread leak in tests.
    
    https://github.com/apache/pulsar/pull/8488 ([@eolivelli](https://github.com/eolivelli))

- [Broker] Cancel the producer's `sendtimeout` task after failing to create the producer.
    
    https://github.com/apache/pulsar/pull/8497 ([@hrsakai](https://github.com/hrsakai))

- [Functions] Fix the issue that overriding `jobName` in Kubernetes runtime with custom runtime options may cause collisions when the same `jobName` is used.  
    
    https://github.com/apache/pulsar/pull/8508 ([@jdbeck](https://github.com/jdbeck))

### Ecosystem

- [Broker] Delete Pulsar adapters.

    https://github.com/apache/pulsar/pull/8480 ([@sijie](https://github.com/sijie))

- [AdminCli] Support examining specific messages by position which is related to the earliest or the latest message.
    
    https://github.com/apache/pulsar/pull/8494 ([@MarvinCai](https://github.com/MarvinCai))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- Apache Pulsar Hackathon

    Sign-up: https://www.eventbrite.com/e/apache-pulsar-hackathon-2021-tickets-143906003731

- Pulsar Virtual Summit North America 2021

    Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021
