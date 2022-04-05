---
title: "2022-01-10-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2022-01-03 ~ 2022-01-09"
date: 2022-01-03 ~ 2022-01-09
description: "This is the Pulsar community weekly update for 2022-01-03 ~ 2022-01-09, with updates on Pulsar client, broker, transactions, and so on."
id: "2022-01-10-pulsar-weekly"
---

# Pulsar Community Weekly Update｜ 2022-01-03 ~ 2022-01-09

This is the Pulsar community weekly update for 2022-01-03 ~ 2022-01-09, with updates on Pulsar client, broker, transactions, and so on.

Great thanks to contributors of the following Github ID who helped build Pulsar during the week: 
[lhotari](https://github.com/lhotari), [Technoboy-](https://github.com/Technoboy-), [baomingyu](https://github.com/baomingyu), [lordcheng10](https://github.com/lordcheng10), [liudezhi2098](https://github.com/liudezhi2098), [k2la](https://github.com/k2la), [codelipenghui](https://github.com/codelipenghui), [Shoothzj](https://github.com/Shoothzj), [casuallc](https://github.com/casuallc), [315157973](https://github.com/315157973), [mattisonchao](https://github.com/mattisonchao), [urfreespace](https://github.com/urfreespace), [rdhabalia](https://github.com/rdhabalia), [pgier](https://github.com/pgier), [michaeljmarshall](https://github.com/michaeljmarshall), [huangdx0726](https://github.com/huangdx0726), [RobertIndie](https://github.com/RobertIndie), [goflutterjava](https://github.com/goflutterjava), [wolfstudy](https://github.com/wolfstudy), [gaozhangmin](https://github.com/gaozhangmin), [kimula](https://github.com/kimula), [yuruguo](https://github.com/yuruguo)

## Pulsar Program Overview
- Github Forks: 2.7k
- Github Stars: 10.6k
- Github Contributors: 513

## Pulsar Updates
### Highlights
- [Broker] Make load-balancer config dynamic for the runtime tuning. 
 <br>https://github.com/apache/pulsar/pull/13074 
 <br>by [rdhabalia](https://github.com/rdhabalia)
- [Security] Allow to config web server's `ciphes` and `protocols`. 
 <br>https://github.com/apache/pulsar/pull/13354 
 <br>by [Shoothzj](https://github.com/Shoothzj)
 
 
### Notable Features
- [Python Client] Support `is_conected` in Python Client. 
 <br>https://github.com/apache/pulsar/pull/13662 
 <br>by [k2la](https://github.com/k2la)
- [Upgrade] Website upgrade.
 <br>https://github.com/apache/pulsar/pull/13660 
 <br>by [urfreespace](https://github.com/urfreespace)

 
### Notable Bug Fix
- [BookKeeper] Fix the issue taht key_shared mode maybe deadlock and with a lot of `CLOSE_WAIT`.
 <br>https://github.com/apache/pulsar/pull/11965 
 <br>by [baomingyu](https://github.com/baomingyu)
- [BookKeeper] Fix the issue that reader skip the remaining compacted data during the topic unloading. 
 https://github.com/apache/pulsar/pull/13629 
 <br>by [codelipenghui](https://github.com/codelipenghui)
- [Client] Added test method in `BacklogQuotaCompatibilityTest`.
 <br>https://github.com/apache/pulsar/pull/13557 
 <br>by [Shoothzj](https://github.com/Shoothzj)
- [Presto] Add dependency management entries to address the dependency issue.
 <br>https://github.com/apache/pulsar/pull/13603 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Fix the issue that Broker health check with `TopicVersion.V2` failed.
 <br>https://github.com/apache/pulsar/pull/13525 
 <br>by [gaozhangmin](https://github.com/gaozhangmin)
- [Pulsarsql] Fix time field use error. 
 <br>https://github.com/apache/pulsar/pull/12249 
 <br>by [casuallc](https://github.com/casuallc)
- [Broker] Fix NPE when unloading namespace bundle. 
 <br>https://github.com/apache/pulsar/pull/13571 
 <br>by [315157973](https://github.com/315157973)
- [Broker] Change `ContextClassLoader` to `NarClassLoader` in `AdditionalServlet`. 
 <br>https://github.com/apache/pulsar/pull/13501 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Client] Avoid repeatly set `startMessageIdData` to null for `ConsumerImpl`. 
 <br>https://github.com/apache/pulsar/pull/13606 
 <br>by [codelipenghui](https://github.com/codelipenghui)
- [Broker] Remove redundant code. 
 <br>https://github.com/apache/pulsar/pull/12653 
 <br>by [huangdx0726](https://github.com/huangdx0726)
- [BookKeeper] Fix the issue that Mockito spy creation fails sporadically and causes an exception and Mockito misuse warning.
 <br>https://github.com/apache/pulsar/pull/13621 
 <br>by [lhotari](https://github.com/lhotari)
- [Test] Upgrade Mockito to 3.12.4.
 <br>https://github.com/apache/pulsar/pull/13622 
 <br>by [lhotari](https://github.com/lhotari)
- [Broker] Fix the issue that `spy(new ServerCnx(pulsar))` is flaky and fails with NPE in the ServerCnx constructor. 
 <br>https://github.com/apache/pulsar/pull/13608 
 <br>by [lhotari](https://github.com/lhotari)
- [Pulsarsql] Bump slf4j from 1.7.25 to 1.7.32. 
 <br>https://github.com/apache/pulsar/pull/13595 
 <br>by [Shoothzj](https://github.com/Shoothzj)
- [Pulsarsql] Upgrade Gson version 2.8.6 to 2.8.9 
 <br>https://github.com/apache/pulsar/pull/13610 
 <br>by [mattisonchao](https://github.com/mattisonchao)
- [Client] Introduce `checkstyle-plugi`n to avoid problems.
 <br>https://github.com/apache/pulsar/pull/13650 
 <br>by [yuruguo](https://github.com/yuruguo)
- [Client] Fix the issue that the `pulsar-client-api` module is not protected by the `checkstyle-plugin`.
 <br>https://github.com/apache/pulsar/pull/13638 
 <br>by [goflutterjava](https://github.com/goflutterjava)
- [Function] Remove unmaintained DC/OS deployment examples. 
 <br>https://github.com/apache/pulsar/pull/13632 
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Admin] Fix the issue that website docs for the tenant admin rest API are incorrect.
 <br>https://github.com/apache/pulsar/pull/13658 
 <br>by [pgier](https://github.com/pgier)
- Update NOTICE from 2021-2022.
 <br>https://github.com/apache/pulsar/pull/13653 
 <br>by [Technoboy-](https://github.com/Technoboy-)
- [Broker] Update log content.
 <br>https://github.com/apache/pulsar/pull/13540 
 <br>by [lordcheng10](https://github.com/lordcheng10)
- [Client] Adjustg md style. 
 <br>https://github.com/apache/pulsar/pull/13615 
 <br>by [liudezhi2098](https://github.com/liudezhi2098)
- Cleanup reference to removed grafana docker image. 
 <br>https://github.com/apache/pulsar/pull/13672 
 <br>by [michaeljmarshall](https://github.com/michaeljmarshall)
- [Client] Fix the documentation for chunked message related stats.
 <br>https://github.com/apache/pulsar/pull/13598 
 <br>by [RobertIndie](https://github.com/RobertIndie)
- [Client] Fix code example of producer for delay message. 
 <br>https://github.com/apache/pulsar/pull/13647 
 <br>by [wolfstudy](https://github.com/wolfstudy)
- [Client] Add notes on worker threads to the document.
 <br>https://github.com/apache/pulsar/pull/13636 
 <br>by [kimula](https://github.com/kimula)

## Blog
- [Happenings in the AP Neighborhood Jan. ‘22](https://medium.com/apache-pulsar-neighborhood/happenings-in-the-ap-neighborhood-jan-22-7e9df18b5a09)
- [Apache Pulsar is #5 in Commits to ASF Projects](https://medium.com/apache-pulsar-neighborhood/apache-pulsar-is-5-in-commits-to-asf-projects-2012ed0ab5c7)

## Events / News
- Survey
    - [[5-Min Survey] New Apache Pulsar Website](https://forms.office.com/pages/responsepage.aspx?id=DQSIkWdsW0yxEjajBLZtrQAAAAAAAAAAAAZAAOjIXw9UMFkzWUM0Q0JVSEtXWVY3SlM0UUMzQkxJVC4u)

- Upcoming events
    - April 8, 2022: Netherlands Apache Pulsar Meetup
        - [Graph-based stream processing with Apache Pulsar](https://www.meetup.com/netherlands-apache-pulsar-meetup/events/284660180/)
    - July 18-20, 2022: JBCNconf
        - [Event Streaming for the Best of All Worlds](https://www.jbcnconf.com/2022/infoTalk.html?id=62324db53a63410bd73c06e4&utm_source=twitter&utm_medium=socialmedia)
