---
title: "2021-08-16-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-08-09 ~ 2021-08-15"
date: 2021-08-09 ~ 2021-08-15
description: "This is the Pulsar community weekly update for 2021-08-09 ~ 2021-08-15, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-08-16-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-08-09 ~ 2021-08-15

This is the Pulsar community weekly update for 2021-08-09 ~ 2021-08-15, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[gaoran10](https://github.com/gaoran10), [hangc0276](https://github.com/hangc0276), [tspannhw](https://github.com/tspannhw), [dlg99](https://github.com/dlg99), [oversearch](https://github.com/oversearch), [freeznet](https://github.com/freeznet), [Jennifer88huang](https://github.com/Jennifer88huang), [timmyyuan](https://github.com/timmyyuan), [Anonymitaet](https://github.com/Anonymitaet), [kaushik-develop](https://github.com/kaushik-develop), [eolivelli](https://github.com/eolivelli), [vroyer](https://github.com/vroyer), [315157973](https://github.com/315157973), [gaozhangmin](https://github.com/gaozhangmin), [jerrypeng](https://github.com/jerrypeng), [BewareMyPower](https://github.com/BewareMyPower), [codelipenghui](https://github.com/codelipenghui), [lhotari](https://github.com/lhotari), [Technoboy-](https://github.com/Technoboy-), [liangyepianzhou](https://github.com/liangyepianzhou), [congbobo184](https://github.com/congbobo184)



## Pulsar Program Overview
- Github Forks: 2.3K
- Github Stars: 9.4K
- Github Contributors: 435

## Pulsar Updates

### Pulsar Highlight
- [Java Client] Produce messages with KeyValue encoding, so that users will be able to set the schema while using `pulsar-client produce`. 
<br>https://github.com/apache/pulsar/pull/11303 
<br>by [eolivelli](https://github.com/eolivelli)

- [Broker] Use the fully-qualified namespace name in register/unregister namespaces to avoid aliasing.
<br>https://github.com/apache/pulsar/pull/11643 
<br>by [kaushik-develop](https://github.com/kaushik-develop)

### Notable Feature
- [Transaction] Fix the issue that Pulsar 2.8.0 cannot be used when transaction is started in standalone mode.
<br>https://github.com/apache/pulsar/pull/11494 
<br>by [liangyepianzhou](https://github.com/liangyepianzhou)

- [Broker] Add metrics for writing or reading size of cursor. 
<br>https://github.com/apache/pulsar/pull/11500 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [Java Client] Remove usage of reflection while using Pulsar Implementation classes. 
<br>https://github.com/apache/pulsar/pull/11636 
<br>by [eolivelli](https://github.com/eolivelli)

### Notable Bug Fix
- [Flaky test] Fix `ManagedLedgerTest.testLedgerReachMaximumRolloverTime`. 
<br>https://github.com/apache/pulsar/pull/11670 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [Broker] Use `getIfValid` to avoid `handleMetadataStoreNotification` swallowing exception. 
<br>https://github.com/apache/pulsar/pull/11656 
<br>by [Technoboy-](https://github.com/Technoboy-)

- [Security] Upgrade Jetty to 9.4.43.v20210629. 
<br>https://github.com/apache/pulsar/pull/11660 
<br>by [lhotari](https://github.com/lhotari)

- [C++ Client] Fix use-after-free and constructor bugs in `UnAckedMessageTrackerEnabled`. 
<br>https://github.com/apache/pulsar/pull/11630 
<br>by [oversearch](https://github.com/oversearch)

- [Transaction] Fix transaction buffer client handle endTxn op when topic or sub are deleted. 
<br>https://github.com/apache/pulsar/pull/11304 
<br>by [congbobo184](https://github.com/congbobo184)

- [Broker] Fix java.lang.NoSuchMethodError with `java.nio.ByteBuffer.position(I)Ljava/nio/ByteBuffer` when enabling topic metadata compression.
<br>https://github.com/apache/pulsar/pull/11594 
<br>by [codelipenghui](https://github.com/codelipenghui)

- [Python Schema] Fix redefined `Record` or `Enum` in Python schema. 
<br>https://github.com/apache/pulsar/pull/11595 
<br>by [gaoran10](https://github.com/gaoran10)

- [Function] Fix the issue that cast exception occurs if function/source/sink type is ByteBuffer. 
<br>https://github.com/apache/pulsar/pull/11611 
<br>by [jerrypeng](https://github.com/jerrypeng)

- [Java Client] Fix the issue that null MessageId may be passed to its compareTo() method. 
<br>https://github.com/apache/pulsar/pull/11607 
<br>by [BewareMyPower](https://github.com/BewareMyPower)

- [Broker] Fix `getPreviousPosition` NPE. 
<br>https://github.com/apache/pulsar/pull/11621 (
<br>by [gaozhangmin](https://github.com/gaozhangmin)

- [Broker] Avoid redundant calls getting the offload policies from offloader. 
<br>https://github.com/apache/pulsar/pull/11629 
<br>by [codelipenghui](https://github.com/codelipenghui)

- [Broker] Use `get` instead of `join` to avoid getting stuck. 
<br>https://github.com/apache/pulsar/pull/11597 
<br>by [315157973](https://github.com/315157973)


## Events / News
- Announcement
    - [Pulsar 2.7.3 release blog](https://streamnative.io/en/blog/release/2021-08-11-pulsar-273/)
    - Welcome [Rui Fu](https://github.com/freeznet) as Apache Pulsar Committer!

- Upcoming Events
    - September 9th: [Webinar Series - Building Microservices with Pulsar](https://streamnative.zoom.us/webinar/register/WN_0vVCCqGhQ4G1978pZvxwZg)
    - September 16th: [Apache Pulsar Deep Dive, an end-to-end view of the data flow](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/280174947/)
    - September 21-23th: [ApacheCon 2021](https://www.apachecon.com/acah2021/)
    - October 6th: [Pulsar Virtual Summit Europe](https://hopin.com/events/pulsar-summit-europe-2021)


## Credits
The Pulsar Weekly is brought to you by [Bo Cong](https://github.com/congbobo184) and [Jipei Wang](https://github.com/JipeiWang)


Thank you for reading. See you next week!


