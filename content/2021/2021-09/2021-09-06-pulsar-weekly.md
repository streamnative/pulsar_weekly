---
title: "2021-09-06-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-08-30 ~ 2021-09-05"
date: 2021-08-30 ~ 2021-09-05
description: "This is the Pulsar community weekly update for 2021-08-30 ~ 2021-09-05, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-09-06-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-08-30 ~ 2021-09-05

This is the Pulsar community weekly update for 2021-08-30 ~ 2021-09-05, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week:
[urfreespace](https://github.com/urfreespace), [gaoran10](https://github.com/gaoran10), [Technoboy-](https://github.com/Technoboy-), [zhanghaou](https://github.com/zhanghaou), [merlimat](https://github.com/merlimat), [BewareMyPower](https://github.com/BewareMyPower), [hangc0276](https://github.com/hangc0276), [sijia-w](https://github.com/sijia-w), [codelipenghui](https://github.com/codelipenghui), [ivankelly](https://github.com/ivankelly), [Shoothzj](https://github.com/Shoothzj), [aloyszhang](https://github.com/aloyszhang), [michaeljmarshall](https://github.com/michaeljmarshall), [nlu90](https://github.com/nlu90), [freeznet](https://github.com/freeznet), [lhotari](https://github.com/lhotari), [congbobo184](https://github.com/congbobo184)


## Pulsar Program Overview
- Github Forks: 2.4k
- Github Stars: 9.5k
- Github Contributors: 447

## Pulsar Updates

### Notable Features

- [Broker] Expose compaction metrics to Prometheus. 
<br>https://github.com/apache/pulsar/pull/11739 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [Metadata] Added MetadataStore `deleteRecursive` operation. 
<br>https://github.com/apache/pulsar/pull/11867 
<br>by [merlimat](https://github.com/merlimat)


- [Logging] Implement structured logging. 
<br>https://github.com/apache/pulsar/pull/11901 
<br>by [ivankelly](https://github.com/ivankelly)

- [Function] Enable protobuf-native schema support for function. 
<br>https://github.com/apache/pulsar/pull/11868 
<br>by [nlu90](https://github.com/nlu90)
 
- [Build] Upgrade Netty to 4.1.67.Final. 
<br>https://github.com/apache/pulsar/pull/11875 
<br>by [lhotari](https://github.com/lhotari)

- [Function] Sync the latest function proto to pulsar-go-function. 
<br>https://github.com/apache/pulsar/pull/11853 
<br>by [freeznet](https://github.com/freeznet)

- [Schema] Config schema compatibility strategy in broker level. 
<br>https://github.com/apache/pulsar/pull/11856 
<br>by [congbobo184](https://github.com/congbobo184)


### Notable Bug Fix

- [Broker] Refine topic level backlog quota policies warning log. 
<br>https://github.com/apache/pulsar/pull/11863 
<br>by [gaoran10](https://github.com/gaoran10)
 
 - [Admin] Fix Pulsar admin method `:getMessageById`. 
<br>https://github.com/apache/pulsar/pull/11852 
<br>by [zhanghaou](https://github.com/zhanghaou)
 
 - [Python] Ensure producer is keeping the client object alive. 
<br>https://github.com/apache/pulsar/pull/11887 
<br>by [merlimat](https://github.com/merlimat)

- [C++] Fix incorrect connect timeout implementation. 
<br>https://github.com/apache/pulsar/pull/11889 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Security] Forbid reading other topic's data in managedLedger layer. 
<br>https://github.com/apache/pulsar/pull/11912 
<br>by [hangc0276](https://github.com/hangc0276)

- [Python] Fix deadlock caused by `ExecutorService::close`. 
<br>https://github.com/apache/pulsar/pull/11882 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Metadata] Fixed merge conflict on `MetadataStoreTest`. 
<br>https://github.com/apache/pulsar/pull/11921 
<br>by [merlimat](https://github.com/merlimat)

- [Tests] Fix proxy flaky test. 
<br>https://github.com/apache/pulsar/pull/11900 
<br>by [codelipenghui](https://github.com/codelipenghui)

- [Client] Remove the uncorrect `VisableTesting` annotation in pulsar-client. 
<br>https://github.com/apache/pulsar/pull/11784 
<br>by [Shoothzj](https://github.com/Shoothzj)
 
 - [Client] Fix receiving duplicated messages after seek at batchIndex level.  
<br>https://github.com/apache/pulsar/pull/11826 
<br>by [aloyszhang](https://github.com/aloyszhang)
 
 - [Security] `AuthorizationService` use provider's `canLookupAsync` method. 
<br>https://github.com/apache/pulsar/pull/11777 
<br>by [michaeljmarshall](https://github.com/michaeljmarshall)

- [Client] Reduce redundant `FLOW `requests for non-durable multi-topics consumer. 
<br>https://github.com/apache/pulsar/pull/11802 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Test] Fix managed cursor metrics test. 
<br>https://github.com/apache/pulsar/pull/11879 
<br>by [gaoran10](https://github.com/gaoran10)

- [Client] Fix the parameter's description in packages client tool. 
<br>https://github.com/apache/pulsar/pull/11809 
<br>by [freeznet](https://github.com/freeznet)

- [Tests] Fixed `ResourceLockTest.revalidateLockOnDifferentSession()`. 
<br>https://github.com/apache/pulsar/pull/11885 
<br>by [merlimat](https://github.com/merlimat)

- [Metadata] Fixed `ZKSessionTest.testReacquireLocksAfterSessionLost`. 
<br>https://github.com/apache/pulsar/pull/11886 
<br>by [merlimat](https://github.com/merlimat)

- [Tests] Fix `BaseMetadataStoreTest` retries .
<br>https://github.com/apache/pulsar/pull/11778 
<br>by [lhotari](https://github.com/lhotari)

- [Function] `ConcurrentHashMap` is used for caching producers. 
<br>https://github.com/apache/pulsar/pull/11820
<br>by [lhotari](https://github.com/lhotari)

## Events / News
- Upcoming Events
    - September 9th: [Webinar Series - Building Microservices with Pulsar](https://streamnative.zoom.us/webinar/register/WN_0vVCCqGhQ4G1978pZvxwZg)
    - September 16th: [Apache Pulsar Deep Dive, an end-to-end view of the data flow](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/280174947/)
    - September 21-23th: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - September 30th: [Apache Pulsar Meetup Japan](https://japan-pulsar-user-group.connpass.com/event/222026/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)

- Call For Participation
    - [Pulsar Summit Asia 2021 CFP is Open until 09/30](https://pulsar.apache.org/blog/2021/08/18/asia-cfp/)