---
title: "2021-09-13-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-09-06 ~ 2021-09-12"
date: 2021-09-06 ~ 2021-09-12
description: "This is the Pulsar community weekly update for 2021-09-06 ~ 2021-09-12, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-09-13-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-09-06 ~ 2021-09-12

This is the Pulsar community weekly update for 2021-09-06 ~ 2021-09-12, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[merlimat](https://github.com/merlimat), [gaozhangmin](https://github.com/gaozhangmin), [hangc0276](https://github.com/hangc0276), [codelipenghui](https://github.com/codelipenghui), [michaeljmarshall](https://github.com/michaeljmarshall), [lhotari](https://github.com/lhotari), [yuruguo](https://github.com/yuruguo), [Shoothzj](https://github.com/Shoothzj), [kaushik-develop](https://github.com/kaushik-develop), [urfreespace](https://github.com/urfreespace), [tuteng](https://github.com/tuteng),  [shibd](https://github.com/shibd), [Technoboy-](https://github.com/Technoboy-), [ivankelly](https://github.com/ivankelly), [gaoran10](https://github.com/gaoran10), [tomscut](https://github.com/tomscut)


## Pulsar Program Overview
- Github Forks: 2.4k
- Github Stars: 9.5k
- Github Contributors: 447

## Pulsar Updates
### Highlights
- [Broker] Add verification when terminating non-persistent topic. 
<br>https://github.com/apache/pulsar/pull/11903 
<br>by [shibd](https://github.com/shibd)

- [Logging] PIP-89: Allow log events to be timed. 
<br>https://github.com/apache/pulsar/pull/11944 
<br>by [ivankelly](https://github.com/ivankelly)

- [C++] Move all C symbols into C++ Pulsar namespace. 
<br>https://github.com/apache/pulsar/pull/11919 
<br>by [merlimat](https://github.com/merlimat)


### Notable Features
- [Python] Expose `Client.shutdown()` method. 
<br>https://github.com/apache/pulsar/pull/11955 
<br>by [merlimat](https://github.com/merlimat)

- [Transaction] Add method to clear up transaction buffer snapshot. 
<br>https://github.com/apache/pulsar/pull/11934 
<br>by [gaoran10](https://github.com/gaoran10)

- [Client] Add an optional params scope for Pulsar Oauth2 Client.
<br>https://github.com/apache/pulsar/pull/11931 
<br>by [tuteng](https://github.com/tuteng)

- [ZooKeeper] Use ZooKeeper "container" types to intermediate z-nodes. 
<br>https://github.com/apache/pulsar/pull/11925 
<br>by [merlimat](https://github.com/merlimat)

- [Builder] Set defaults on fields in `TopicPolicies` and `Actions` classes.
<br>https://github.com/apache/pulsar/pull/12009 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

- [Schema] Remove unnecessary creation of `JsonParser` object per deprecation doc. 
<br>https://github.com/apache/pulsar/pull/12008 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

### Notable Bug Fix

- [C++] Fixed attemptions to connect to multiple IP address. 
<br>https://github.com/apache/pulsar/pull/11958
<br>by [merlimat](https://github.com/merlimat)

- [BookKeeper] Print position info when can't find a next valid position. 
<br>https://github.com/apache/pulsar/pull/11969 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [C++] Handle error when shutting down client after forks. 
<br>https://github.com/apache/pulsar/pull/11954 
<br>by [merlimat](https://github.com/merlimat)

- [Client] Fix the issue that forget to call `SendCallback` on producer close. 
<br>https://github.com/apache/pulsar/pull/11939 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [Broker] Avoid infinitely splitting bundle when there is only one topic. 
<br>https://github.com/apache/pulsar/pull/11937 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [Test] Add date for the logs by default. 
<br>https://github.com/apache/pulsar/pull/11935 
<br>by [tomscut](https://github.com/tomscut)

- [Client] Fix the issue that the client doesn't update memory counter when closing a producer.
<br>https://github.com/apache/pulsar/pull/11906 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [BookKeeper](/3PIwqftdRmer7Knitp7SxQ) Remove tiny size of deprecated Netty allocator. 
<br>https://github.com/apache/pulsar/pull/12012 
<br>by [Shoothzj](https://github.com/Shoothzj)

- [ZooKeeper] Fix String formatting conversion in `toString` method. 
<br>https://github.com/apache/pulsar/pull/12006 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

- [Standalone] Fix the assignment of a custom stream-storage-port number 
<br>https://github.com/apache/pulsar/pull/11995 
<br>by [lhotari](https://github.com/lhotari)

- Remove unused variable and unneccessary box in NamespaceBundleFactory 
https://github.com/apache/pulsar/pull/11975 
by [Shoothzj](https://github.com/Shoothzj)

- [Broker] Remove unnecessary boxing. 
<br>https://github.com/apache/pulsar/pull/11994 
<br>by [lhotari](https://github.com/lhotari)

- [Test] Add breaks to prevent fall through in MockZooKeeper. 
<br>https://github.com/apache/pulsar/pull/12007 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

## Blog
- [Speakers Announced for Pulsar Virtual Summit Europe 2021](https://streamnative.io/blog/community/2021-09-07-speakers-announced-for-pulsar-virtual-summit-europe-2021/)

## Events / News
- Past Events
    - [Developing Event-driven Microservices using Apache Pulsar](https://www.youtube.com/watch?v=hI1Y_qMilsA&list=PLqRma1oIkcWhfmUuJrMM5YIG8hjju62Ev&index=3)
- Upcoming Events
    - September 16th: [Apache Pulsar Deep Dive, an end-to-end view of the data flow](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/280174947/)
    - September 21-23th: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - September 30th: [Apache Pulsar Meetup Japan](https://japan-pulsar-user-group.connpass.com/event/222026/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)

- Call For Participation
    - [Pulsar Summit Asia 2021 CFP is Open until 09/30](https://pulsar.apache.org/blog/2021/08/18/asia-cfp/)