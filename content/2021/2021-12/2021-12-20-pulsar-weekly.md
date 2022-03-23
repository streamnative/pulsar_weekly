---
title: "2021-12-20-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-12-13 ~ 2021-12-19"
date: 2021-12-13 ~ 2021-12-19
description: "This is the Pulsar community weekly update for 2021-12-13 ~ 2021-12-19, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-12-20-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2021-12-13 ~ 2021-12-19

This is the Pulsar community weekly update for 2021-12-13 ~ 2021-12-19, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[aloyszhang](https://github.com/aloyszhang), [eolivelli](https://github.com/eolivelli), [yuruguo](https://github.com/yuruguo), [315157973](https://github.com/315157973), [Demogorgon314](https://github.com/Demogorgon314), [BewareMyPower](https://github.com/BewareMyPower), [Technoboy-](https://github.com/Technoboy-), [Shoothzj](https://github.com/Shoothzj), [wuzhanpeng](https://github.com/wuzhanpeng), [nicoloboschi](https://github.com/nicoloboschi), [LeBW](https://github.com/LeBW), [liangyepianzhou](https://github.com/liangyepianzhou), [gaoran10](https://github.com/gaoran10), [lhotari](https://github.com/lhotari), [ericsyh](https://github.com/ericsyh), [HQebupt](https://github.com/HQebupt), [urfreespace](https://github.com/urfreespace), [codelipenghui](https://github.com/codelipenghui)

## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.4k
- Github Contributors: 513

## Pulsar Updates
### Highlights
- [Broker] Support global topic policy and local topic policy.
 <br>https://github.com/apache/pulsar/pull/12517 
 <br>by [315157973](https://github.com/315157973)
- [Pulsar Client] Support querying chunked messages feature in Pulsar SQL.
 <br>https://github.com/apache/pulsar/pull/12720 
 <br>by [gaoran10](https://github.com/gaoran10)
- [Security] Upgrade to Log4J 2.17.0 to mitigate CVE-2021-45105.
 <br>https://github.com/apache/pulsar/pull/13392 
 <br>by [lhotari](https://github.com/lhotari)
 
### Notable Features
- [Function] Add a new configuration parameter `additionalJavaRuntimeArguments` to `functions_worker.conf`.
 <br>https://github.com/apache/pulsar/pull/13282 
 <br>by [eolivelli](https://github.com/eolivelli)
- [C++ Client] Support more Pulsar command name and version in Wireshark dissector. 
 <br>https://github.com/apache/pulsar/pull/13286 
 <br>by [Demogorgon314](https://github.com/Demogorgon314)
- [Broker] Modify return result of `NamespacesBase#internalGetPublishRate`. 
 <br>https://github.com/apache/pulsar/pull/13237 
 <br>by [yuruguo](https://github.com/yuruguo)
- [Admin]  Add description for the `earliestMsgPublishTimeInBacklog` in pulsar-admin.
 <br>https://github.com/apache/pulsar/pull/13263 
 <br>by [LeBW](https://github.com/LeBW)
- [Transaction] Add a test in TransactionEndToEndTest.
 <br>https://github.com/apache/pulsar/pull/12521 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] Stop TP replaying with Exception.
 <br>https://github.com/apache/pulsar/pull/12700 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] Allow `abort` or `commit` in the state of aborting or committing.
 <br>https://github.com/apache/pulsar/pull/13323 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] Remove request if can not be sent. 
 <br>https://github.com/apache/pulsar/pull/13308 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Admin] Add replicated subscriptions limitations of `markDeletePosition` sync.
 <br>https://github.com/apache/pulsar/pull/13230 
 <br>by [ericsyh](https://github.com/ericsyh)
 
### Notable Bug Fix
- [Broker] Fix the issue that topic Lookup on non-existent topics return unexpected response.
 <br>https://github.com/apache/pulsar/pull/13055 
 <br>by [aloyszhang](https://github.com/aloyszhang)
- [Authorization] Converge authz of namespace policies from super-user to tenant-administrator. 
 <br>https://github.com/apache/pulsar/pull/13157 
 <br>by [yuruguo](https://github.com/yuruguo)
- [C++ Client] Fix the issue that `Version.h` cannot be found when CMake binary directory is customized. 
 <br>https://github.com/apache/pulsar/pull/13324 
 <br>by [BewareMyPower](https://github.com/BewareMyPower)
- [Broker] Close old compacted ledger when open new. 
 <br>https://github.com/apache/pulsar/pull/13210 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Pulsar Client] Call `triggerListener` always in `internalPinnedExecutor`.
 <br>https://github.com/apache/pulsar/pull/13023 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Common] Fix the issue that Cipher parameter not work in `KeyStoreSSLContext`. 
 <br>https://github.com/apache/pulsar/pull/13322 
 <br>by [Shoothzj](https://github.com/Shoothzj)
- [Broker] Fix the pattern matching problem and add a test case for it.
 <br>https://github.com/apache/pulsar/pull/13208 
 <br>by [wuzhanpeng](https://github.com/wuzhanpeng)
- [Owasp] Add the suppression for this jar as in the owasp plugin repository.
 <br>https://github.com/apache/pulsar/pull/13364 
 <br>by [nicoloboschi](https://github.com/nicoloboschi)
- [Transaction] Delete the redundant code.
 <br>https://github.com/apache/pulsar/pull/13327 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Transaction] Fix the issue that no `TransactionCoordinatorNotFound`, but automatic reconnect. 
 <br>https://github.com/apache/pulsar/pull/13135 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou) 
- [Transaction] Fix the issue that there is one omission and several irregular log formats. 
 <br>https://github.com/apache/pulsar/pull/13253 
 <br>by [liangyepianzhou](https://github.com/liangyepianzhou)
- [Function] Make the unit test and integration test work 
 <br>https://github.com/apache/pulsar/pull/13243 
 <br>by [codelipenghui](https://github.com/codelipenghui)
 

## Resources 
### Blog
- [Building Edge Applications With Apache Pulsar](https://dev.to/tspannhw/building-edge-applications-with-apache-pulsar-1ff2)
- [Developing Event-Driven Microservices with Apache Pulsar: Part I](https://streamnative.io/blog/engineering/2021-12-14-developing-event-driven-microservices-with-apache-pulsar/)
- [What’s New in Apache Pulsar 2.7.4](https://streamnative.io/blog/release/2021-12-14-pulsar-274/) 

### Video
- [Hail Hydrate! From Stream to Lake with Pulsar and Friends](https://www.youtube.com/watch?v=vDfKKNLypnA)

## Events
- Upcoming events
    - March 21-25, 2022: The 4th annual 2022 Python Web Conference
        - [The most in-depth Python conference for web developers](https://2022.pythonwebconf.com/)
    - March 23, 2022: Live Webinar
        - [Event Streaming with Apache Pulsar and Kotlin](https://info.jetbrains.com/kotlin-webinar-march22-2022.html?)
    - March 29, 2022: Webinar
        - How to Build an Event Sourcing App with Apache Pulsar
    - March 30, 2022: Open Source Bristol
        - [Building a Scalable Event Streaming and Messaging Platform using Apache Pulsar for Fintech](https://www.meetup.com/Open-Source-Bristol/events/284198269/)
    - April 8, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)