---
title: "2021-11-22-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-11-15 ~ 2021-11-21"
date: 2021-11-15 ~ 2021-11-21
description: "This is the Pulsar community weekly update for 2021-11-15 ~ 2021-11-21, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-11-22-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-11-15 ~ 2021-11-21

This is the Pulsar community weekly update for 2021-11-15 ~ 2021-11-21, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: [casuallc](https://github.com/casuallc), [codelipenghui](https://github.com/codelipenghui), [Jason918](https://github.com/Jason918), [mingyifei](https://github.com/mingyifei), [merlimat](https://github.com/merlimat), [liangyepianzhou](https://github.com/liangyepianzhou), [nlu90](https://github.com/nlu90), [nicoloboschi](https://github.com/nicoloboschi), [Technoboy-](https://github.com/Technoboy-), [yuruguo](https://github.com/yuruguo), [freeznet](https://github.com/freeznet), [zeo1995](https://github.com/zeo1995), [eolivelli](https://github.com/eolivelli), [lhotari](https://github.com/lhotari), [Shoothzj](https://github.com/Shoothzj), [urfreespace](https://github.com/urfreespace)

## Pulsar Program Overview
- Github Forks: 2.5k
- Github Stars: 10k
- Github Contributors: 465

## Pulsar Updates

### Highlights.
- [Broker] Check service status before `Pulsar-Admin` runs commands.
<br>https://github.com/apache/pulsar/pull/12847 <br>by [freeznet](https://github.com/freeznet)

### Notable Features
- [Test] Support `listenerThreads` configuration. 
<br>https://github.com/apache/pulsar/pull/12892 <br>by [mingyifei](https://github.com/mingyifei)

- [Metadata] Remove unneeded ZooKeeper operations. 
<br>https://github.com/apache/pulsar/pull/12866 <br>by [merlimat](https://github.com/merlimat)

- [Broker] Support roles with `consume` topic authorization to `GET_BACKLOG_SIZE` of the topic.
<br>https://github.com/apache/pulsar/pull/12850 <br>by [yuruguo](https://github.com/yuruguo)

- [BookKeeper] Catch exceptions in scheduled tasks to prevent unintended cancellation. 
<br>https://github.com/apache/pulsar/pull/12853 <br>by [lhotari](https://github.com/lhotari)
 
### Notable Bug Fix
 - [BookKeeper] Fix the issue that the exception is handled twice repeatedly.
<br>https://github.com/apache/pulsar/pull/12881 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)

- [Transaction] Stop `MLTransactionLogImpl` from constantly replaying.
<br>https://github.com/apache/pulsar/pull/12705 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)

- [Broker] Fix the issue that broker from removed-cluster fails to unload topic and namespace.
<br>https://github.com/apache/pulsar/pull/12583 <br>by [Technoboy-](https://github.com/Technoboy-)

- [Broker]  Fix the issue that when deleting tenants with active namespaces unexpected response code is returned.
<br>https://github.com/apache/pulsar/pull/12848 <br>by [Technoboy-](https://github.com/Technoboy-)

- [Broker] Remove the key from `listeners` if the value list is empty.
<br>https://github.com/apache/pulsar/pull/12654 <br>by [Jason918](https://github.com/Jason918)

- [Broker] Add two configurations options to create a dedicate `EventLoopGroup` for per each Protocol Handler and Proxy Extensions.
<br>https://github.com/apache/pulsar/pull/12692 <br>by [eolivelli](https://github.com/eolivelli)
 
## Blog
- [No Time to Waste: 100,000 Messages a Second and Growing](https://www.rtinsights.com/no-time-to-waste-100000-messages-a-second-and-growing/)
- [Building Edge Applications With Apache Pulsar](https://streamnative.io/blog/engineering/2021-11-17-building-edge-applications-with-apache-pulsar/)

## Events / News
- Past Events
    - Porto Tech Hub Conference 2021
        - [Hail Hydrate! From Stream to Lake with Apache Pulsar and Friends](https://www.youtube.com/watch?v=K9MOiG1oz-0&t=6s)
- Upcoming Events
    - December 3rd: Embedded Fest ONLINE
        - [Using Apache Pulsar to provide real-time analytics on the edge](https://embeddedfest.com/)
    - December 9th: [Virtual Book Launch: Apache Pulsar in Action](https://streamnative.io/event/webinar-book-launch/)