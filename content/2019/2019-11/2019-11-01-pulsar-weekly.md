---
title: "2019-11-01-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-10-26 ~ 2019-11-01"
date: 2019-10-26 ~ 2019-11-01
description: "This is the Pulsar community weekly update for 2019-10-26 ~ 2019-11-01, with updates on new PIPs kicking in discussions of revisiting admin API and permissions, introducing package management in Pulsar Functions, a new Pulsar admin CLI `pulsarctl`, first apache release of Pulsar Manager, and a bit more."
---


## [Pulsar Community Weekly Update] 2019-10-26 ~ 2019-11-01 

This is the Pulsar community weekly update for 2019-10-26 ~ 2019-11-01, with updates on new PIPs kicking in discussions of revisiting admin API and permissions, introducing package management in Pulsar Functions, a new Pulsar admin CLI `pulsarctl`, first apache release of Pulsar Manager, and a bit more.

### Pulsar Development

- [Pulsar Manager] The release plan was settled down. Guangning is going to kick off the first release plan.

    https://lists.apache.org/thread.html/b3f05f0f50a6b8c32536c5a29f8e1ce5c6efe42b2a6ccf91f28d33a0@%3Cdev.pulsar.apache.org%3E

- [PIP-47][Release] Time-Based Release Plan

    PIP-47 was submitted for proposing moving towards a time-based release plan. So Pulsar development can enter a faster feedback cycle and users can benefit from features shipped quicker.

    - https://lists.apache.org/thread.html/6509f012d52241090dd987609ed7eb27ab29af224217f6934cfee64c@%3Cdev.pulsar.apache.org%3E
  
    - https://github.com/apache/pulsar/wiki/PIP-47%3A-Time-Based-Release-Plan


- [PIP-48][admin] Hierarchical admin API

    Steven and Florentin from OVH kicked off a discussion for improving current admin API.

    - https://lists.apache.org/thread.html/742ff9ffcc1f7212acf5e0eaae4bbd45c4754a43b7a36f22bd57578a@%3Cdev.pulsar.apache.org%3E
  
    - https://github.com/apache/pulsar/wiki/PIP-48%3A-hierarchical-admin-api

- [PIP-49][admin] Permission levels and inheritance

    Xiaolong started a proposal for revisiting the permission levels and inheritance in the Pulsar admin API.
    
    - https://lists.apache.org/thread.html/d56048b007d713d7b927c37e4cdf23a353852b2f7d6491840f1e3e0f@%3Cdev.pulsar.apache.org%3E
  
    - https://github.com/apache/pulsar/wiki/PIP-49%3A-Permission-levels-and-inheritance

- [PIP-50][Functions] Package Management

    Yong proposed introducing a package management system for managing different versions of functions and connectors.

    - https://lists.apache.org/thread.html/61a8138b0a304298d0de6178c5b870b38bd32bd762374486777f2c8c@%3Cdev.pulsar.apache.org%3E
  
    - https://github.com/apache/pulsar/wiki/PIP-50%3A-Package-Management


- [Document] The broken links in the website have been fixed. Kudos to Guangning and Jennifer.

- [Document] A new discussion thread started to introduce versioning in managing Pulsar client API documentation.

- [Functions] Distributed the CA for KubernetesSecretsTokenAuthProvider (Release: 2.5.0)

    - https://github.com/apache/pulsar/pull/5469

    - https://lists.apache.org/thread.html/a6a91990907cf8d2458ff8b7e1e916a9bfb17ec0cd216d57c66ab96c@%3Cdev.pulsar.apache.org%3E


- [BookKeeper] Apache BookKeeper is voting its 4.10 release, which can unblock Pulsar 2.4.2 release. Thank you to Enrico from the BookKeeper community!

    https://lists.apache.org/thread.html/d57f500fe8383903922fc4be3c3901fb0c00fda777672f32653c979e@%3Cdev.bookkeeper.apache.org%3E

### Notable Features

- [Functions] Added deletion of state for Functions (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5469
    
    
- [Functions] Distributed the CA for KubernetesSecretsTokenAuthProvider (Release: 2.5.0)

    https://github.com/apache/pulsar/pull/5398
    
- [ZooKeeper] Bumped ZooKeeper to version 3.5.6

    https://github.com/apache/pulsar/pull/5043
    
- [Functions] Function runtime pluggable

    https://github.com/apache/pulsar/pull/5463


### Notable Bug Fix

- [Client][Java] Wrongly report "3600 messages have timed-out" (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5477
    
- [Functions] Fixed Pulsar can not load the customized SerDe (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5357
    
- [Authentication] Fixed broken custom auth-provider that uses authenticationData (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5462
    
- [Tiered Storage] Only seek when reading unexpected entry (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5356
    
- [Broker] Trim messages which less than mark delete position for message redelivery (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5378
    
- [Admin] Fix list non-persistent topics shows the persistent topics (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5502

### Ecosystem

- [CLI] StreamNative open sourced a Pulsar Go admin client and a new CLI tool `pulsarctl` (built on the Pulsar Go admin client).

    https://github.com/streamnative/pulsarctl
    
    
- [Hadoop-unit](https://github.com/jetoile/hadoop-unit) added the support for Pulsar and BookKeeper.

    https://github.com/jetoile/hadoop-unit/blob/master/CHANGELOG.md#v36-20191101-1603-0000
    
- Pulsar.Client 0.8.0 was released with Reader support.

    https://www.nuget.org/packages/Pulsar.Client/
    

### Event/News

- [Meetup] A new Apache Pulsar meetup is coming in Shanghai (China) on November 16, which will feature adoption stories from China Telecom, Zhaopin, and TuyaSmart.

    Signup link: https://www.eventbrite.com/e/apache-pulsar-meetup-shanghai-tickets-79293658467


### Blog/Article

- [Video] Presentation "Apache Pulsar 101: architecture, concepts et comparaison" given by Quentin Adam & Steven Le Roux at DevFest Nantes 2019 was alive.

    https://www.youtube.com/watch?v=5fqhT82wghY&list=PLuZ_sYdawLiUjPGPsOvBcgBxC6yP_HSA6&index=55&t=0s
