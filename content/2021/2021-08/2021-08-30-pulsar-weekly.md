---
title: "2021-08-30-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-08-23 ~ 2021-08-29"
date: 2021-08-23 ~ 2021-08-29
description: "This is the Pulsar community weekly update for 2021-08-23 ~ 2021-08-29, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-08-30-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-08-23 ~ 2021-08-29

This is the Pulsar community weekly update for 2021-08-23 ~ 2021-08-29, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[sijia-w](https://github.com/sijia-w), [merlimat](https://github.com/merlimat), [ivankelly](https://github.com/ivankelly), [lhotari](https://github.com/lhotari), [hangc0276](https://github.com/hangc0276), [freeznet](https://github.com/freeznet), [michaeljmarshall](https://github.com/michaeljmarshall), [michaeljmarshall](https://github.com/michaeljmarshall), [Anonymitaet](https://github.com/Anonymitaet), [urfreespace](https://github.com/urfreespace), [Nicklee007](https://github.com/Nicklee007), [codelipenghui](https://github.com/codelipenghui), [Shoothzj](https://github.com/Shoothzj), [gaozhangmin](https://github.com/gaozhangmin), [nemecec](https://github.com/nemecec), [dave2wave](https://github.com/dave2wave), [nicoloboschi](https://github.com/nicoloboschi), [BewareMyPower](https://github.com/BewareMyPower)


## Pulsar Program Overview
- Github Forks: 2.4k
- Github Stars: 9.5k
- Github Contributors: 445

## Pulsar Updates

### Notable Features
- [Java] Adjust interface for structured event logging. 
<br>https://github.com/apache/pulsar/pull/11800 
<br>by [ivankelly](https://github.com/ivankelly)
- [Website] Upgrade the initial framework of Pulsar website.
<br>https://github.com/apache/pulsar/pull/11770 
<br>by [urfreespace](https://github.com/urfreespace)
- [Broker] Upgrade Air Compressor to 0.20.
<br>https://github.com/apache/pulsar/pull/11790 
<br>by [hangc0276](https://github.com/hangc0276)
- [Broker] Revert PR-11594 to avoid copying data to direct buffer. 
<br>https://github.com/apache/pulsar/pull/11792 
<br>by [hangc0276](https://github.com/hangc0276)
- [Test] Use TestRetrySupport for `BaseMetadataStoreTests` to cleanup state between retries.
<br>https://github.com/apache/pulsar/pull/11771 
<br>by [lhotari](https://github.com/lhotari)
- [Function] Support KEY_BASED batch builder for Java based functions and sources. 
<br>https://github.com/apache/pulsar/pull/11706 
<br>by [lhotari](https://github.com/lhotari)


### Notable Bug Fix
- [Client] Fix accessing `MessageImpl` after it was enqueued on user queue. 
<br>https://github.com/apache/pulsar/pull/11824
<br>by [merlimat](https://github.com/merlimat)
- [Build] Fix java_test_functions build fail. 
<br>https://github.com/apache/pulsar/pull/11829 
<br>by [hangc0276](https://github.com/hangc0276)
- [Admin] Cleanup Znode data when namespace is deleted. 
<br>https://github.com/apache/pulsar/pull/11791 
<br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Tests] Fix flaky test `testReacquireLocksAfterSessionLost`. 
<br>https://github.com/apache/pulsar/pull/11815 
<br>by [hangc0276](https://github.com/hangc0276)
- [Broker] Fix the issue that producer close triggers a removal from the map. 
<br>https://github.com/apache/pulsar/pull/11804 
<br>by [merlimat](https://github.com/merlimat)
- [Package Management] Fix `wrappedBuffer` which is always using the same block of memory.  
<br>https://github.com/apache/pulsar/pull/11782 
<br>by [freeznet](https://github.com/freeznet)
- [Build] Fix running `mvn install -DskipTests` from `pulsar/pulsar-broker` and `pulsar/pulsar-transaction/coordinator` fail. 
<br>https://github.com/apache/pulsar/pull/11795 
<br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Client] Fixed race condition on multi-topic consumers. 
<br>https://github.com/apache/pulsar/pull/11764 
<br>by [merlimat](https://github.com/merlimat)
- [Broker] Release memory when sending message timeout. 
<br>https://github.com/apache/pulsar/pull/11761 
<br>by [Shoothzj](https://github.com/Shoothzj)
- [Admin] Fix the bug that topic cannot be updated when the updated topic name is contained by an existed topic. 
<br>https://github.com/apache/pulsar/pull/11686 
<br>by [Nicklee007](https://github.com/Nicklee007)
- [C++] Make some clean up methods thread safe. 
<br>https://github.com/apache/pulsar/pull/11762 
<br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Broker] Fix the topic in fenced state and the issue that topic cannot recover. 
<br>https://github.com/apache/pulsar/pull/11737
<br>by [codelipenghui](https://github.com/codelipenghui)
- [Broker] Call `.release()` when discarding entry to prevent direct memory leak. 
<br>https://github.com/apache/pulsar/pull/11748 
<br>by [lhotari](https://github.com/lhotari)

## Blog
<<<<<<< Updated upstream
- [Scalable Stream Processing with Pulsar’s Key_Shared Subscription](https://streamnative.io/en/blog/engineering/2021-08-25-scalable-stream-processing-with-pulsars-key-shared-subscription/
=======
- [Scalable Stream Processing with Pulsar’s Key_Shared Subscription](https://streamnative.io/en/blog/engineering/2021-08-25-scalable-stream-processing-with-pulsars-key-shared-subscription/)
>>>>>>> Stashed changes

## Events / News
- Upcoming Events
    - September 9th: [Webinar Series - Building Microservices with Pulsar](https://streamnative.zoom.us/webinar/register/WN_0vVCCqGhQ4G1978pZvxwZg)
    - September 16th: [Apache Pulsar Deep Dive, an end-to-end view of the data flow](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/280174947/)
    - September 21-23th: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - September 30th: [Apache Pulsar Meetup Japan](https://japan-pulsar-user-group.connpass.com/event/222026/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)

- Call For Participation
    - [Pulsar Summit Asia 2021 CFP is Open until 09/30](https://pulsar.apache.org/blog/2021/08/18/asia-cfp/)
