---
title: "2019-11-29-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2019-11-23 ~ 2019-11-29"
date: 2019-11-23 ~ 2019-11-29
description: "This is the weekly community update for 2019-11-23 ~ 2019-11-29, with updates on Pulsar user conference @PulsarSummit, Pulsar Manager 0.1.0 release, broker-level publish rate limiting and many other enhancements around metrics and documentation."
---

## [Community Weekly Update] 

This is the weekly community update for 2019-11-23 ~ 2019-11-29, with updates on Pulsar user conference @PulsarSummit, Pulsar Manager 0.1.0 release, broker-level publish rate limiting and many other enhancements around metrics and documentation.

### Pulsar Development

- [Pulsar Manager] Pulsar Manager 0.1.0 is released. It is the first official apache release since it is donated from StreamNative. Thanks to many committers and contributors for making this happen.

    - Release Notes
    
        http://pulsar.apache.org/en/pulsar-manager-release-notes/#010-mdash-2019-11-25-a-id010a
    
    - Documentation

        http://pulsar.apache.org/docs/en/next/administration-pulsar-manager/
    
- [Pulsar][Release] Pulsar 2.4.2 release RC 3 is out for voting.

    https://lists.apache.org/thread.html/3e61e3e2e75fb3b096744bdb9fb5b16399611c8b5cee4a7b1a95c4de@%3Cdev.pulsar.apache.org%3E
    
- [Pulsar][Release] Pulsar 2.5.0 release is progressing. There are a few documentation issues to close. The first release candidate is expected to be out for voting.

    https://github.com/apache/pulsar/milestone/22
    
- [PIP] Alexandre is proposing adding tenant-level policy.

    https://lists.apache.org/thread.html/a937326861b8e49fdb9fc8982010f41fb978a88311ebeb0f24bb695f@%3Cdev.pulsar.apache.org%3E

### Notable Feature

- [Metrics] Expose lastExpireTimestamp for subscription stats (Release: 2.4.3, 2.5.0).

    https://github.com/apache/pulsar/pull/5721
    
- [Broker] A broker level publisher rate limiting mechanism is introduced for preventing broker OOM.

    https://github.com/apache/pulsar/pull/5710
    
- [SQL] Pulsar SQL supports zookeeper chroot (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5001
    
- [Broker] Remove cursor while remove non-durable subscription (Release: 2.5.0).

    https://github.com/apache/pulsar/pull/5719
    

### Notable Bug Fix

- [Java][Client] Fix potential deadlock in pulsar client close (Release: 2.4.3, 2.5.0).

    https://github.com/apache/pulsar/pull/5731


### Ecosystem

- [Flink] Pulsar-Flink connector is submitted to the Flink Packages website.

    https://flink-packages.org/packages/pulsar-flink-connector


### Event/News

- [Conference] Two Pulsar dedicated events "Pulsar Summit San Francisco" and "Pulsar Summit Beijing" are coming 2020. The Call-For-Presentations is open soon.

    https://lists.apache.org/thread.html/458be6deeb0260591a353cf0a252d7d0a892cd662834db585069a3de@%3Cdev.pulsar.apache.org%3E

- [Conference] Flink Forward Asia was held on November 28-30. Yijie Shen attended this conference and gave a speech about the Unified Data Process using Pulsar and Flink.

    https://developer.aliyun.com/special/ffa2019-conference

- [Meetup] The first Apache Pulsar x PingCAP infra meetup happened on November 30. Penghui Li and Yong Zhang presented this meetup and shared everything about Pulsar transactions.

    https://www.huodongxing.com/event/7520647658000
