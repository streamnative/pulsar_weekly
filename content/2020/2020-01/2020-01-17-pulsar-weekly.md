---
title: "2020-01-17-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-01-11 ~ 2020-01-17"
date: 2020-01-11 ~ 2020-01-17
description: "This is the Pulsar community weekly update for 2020-01-11 ~ 2020-01-17, with updates on 2.5.0 release and new proposals about refreshing authentication credentials and message acknowledgment with batches."
---

## [Pulsar Community Weekly Update] 2020-01-11 ~ 2020-01-17

This is the Pulsar community weekly update for 2020-01-11 ~ 2020-01-17, with updates on 2.5.0 release and new proposals about refreshing authentication credentials and message acknowledgment with batches. 

### Development

- [Release] Pulsar 2.5.0 is released!

    http://pulsar.apache.org/release-notes/#250-mdash-2019-12-06-a-id250a
    
- [Release] Sijie Guo raised a discussion to introduce release labels for managing minor releases. The vote is in progress.
  
    https://lists.apache.org/thread.html/ra057f9bb3385f62a9216a202260805074c3f1af77c144907fa1b50cd%40%3Cdev.pulsar.apache.org%3E

- [Release] The community is discussing a 2.4.3 bug fix release.

    https://lists.apache.org/thread.html/rff2325c7f73dd73624595087ab3b2928b456f1faa14294c98d38759c%40%3Cdev.pulsar.apache.org%3E
    
- [BookKeeper] BookKeeper community is discussing abstracting bookie network address from ledger metadata.

    https://lists.apache.org/thread.html/r415c1ed3881714568e88b559fa09fe3816dc5891ca0b73278045cd83%40%3Cdev.pulsar.apache.org%3E
    
- [CI] GitHub action based CI has matured quite a bit. The community is voting for migrating CI from Jenkins to GitHub actions.

    https://lists.apache.org/thread.html/r1e85dca5bb502e113da1a51a3c9308d73dcb50a88fca5cf3684e109b%40%3Cdev.pulsar.apache.org%3E
    
- [PIP-54] Acknowledgement for local index of batch message

    https://github.com/apache/pulsar/wiki/PIP-54:-Acknowledgement-for-local-index-of-batch-message
    
- [PIP-55] Refresh authentication credentials

    https://github.com/apache/pulsar/wiki/PIP-55%3A-Refresh-Authentication-Credentials

### Notable Feature

- [Go Functions] Replace cgo client with native Go client in Go Function

    https://github.com/apache/pulsar/pull/6059
    
- [Broker] Support delete inactive topic when subscriptions caught up

    https://github.com/apache/pulsar/pull/6077

### Notable Bug Fix

- [Client][Java] Fix zero queue consumer message redelivery

    https://github.com/apache/pulsar/pull/6076
    
- [Client][Java] Fix message redelivery for zero queue consumer while using async API to receive messages

    https://github.com/apache/pulsar/pull/6090

### Event / News

- A Pulsar meetup was held on Jan 15 in Toronto. Cory Darby gave a talk about "RIP Apache Kafka, long live Apache Pulsar" and Tamer A shared about "Pulsar in Action, getting your hands dirty with Pulsar".

    https://www.meetup.com/Tech-At-Scale-Toronto-Meetup/events/267651296/
    
    https://www.youtube.com/watch?time_continue=5&v=jLruEmh3ve0&feature=emb_logo

### Blog / Article
    
- Pulsar-express, a web interface for Apache Pulsar (by Bruno Bonnin)

    https://dev.to/bbonnin/pulsar-express-a-web-interface-for-apache-pulsar-1lm