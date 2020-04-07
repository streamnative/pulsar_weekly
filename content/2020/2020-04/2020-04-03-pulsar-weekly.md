---
title: "2020-04-03-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-03-21 ~ 2020-04-03"
date: 2020-03-21 ~ 2020-04-03
description: "This is the Pulsar community weekly update for 2020-03-21 ~ 2020-04-03, with updates on Pulsar 2.5.1 release candidate, native Go client 0.1.0 release, Kafka-on-Pulsar, multiple PIPs, and bug fixes."
id: "2020-04-03-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-03-21 ~ 2020-04-03

This is the Pulsar community weekly update for 2020-03-21 ~ 2020-04-03, with updates on Pulsar 2.5.1 release candidate, native Go client 0.1.0 release, Kafka-on-Pulsar, multiple PIPs, and bug fixes.

### Development

- [Release] The first release candidate of Pulsar 2.5.1 is out for voting.

    https://lists.apache.org/thread.html/rd0781410d7e465cc2c34c04797e6da8079458985b9d3658c8f19ea33%40%3Cdev.pulsar.apache.org%3E

- [Client] Pulsar Native Go Client 0.1.0 is released.

    https://lists.apache.org/thread.html/reac88dbfbade09a2e849c6ae3ec4b295f4ed36160dd34a6b3b9ac742%40%3Cdev.pulsar.apache.org%3E
    
- [PIP-61] Support multiple advertised addresses on broker.

   https://github.com/apache/pulsar/wiki/PIP-61%3A-Advertised-multiple-addresses https://lists.apache.org/thread.html/r007ce702976133f5cc7e97109cdd58d91ca9fd62d146f06523a18c1e%40%3Cdev.pulsar.apache.org%3E

- [Pulsar-Flink] Discussion in the community to deprecate the Flink 1.6.0 integration as a newer Flink connector is proposed to Flink upstream in FLIP-72.

    https://lists.apache.org/thread.html/r1772fc6a326dde79312362d16be96acaf9095ccc0ee7234b1ffe8618%40%3Cdev.pulsar.apache.org%3E

### Notable Feature

- [Broker] Namespace policy overrides (Release: 2.6.0).
  
    - AutoTopicCreation: https://github.com/apache/pulsar/pull/6471
  
    - Offload policies: https://github.com/apache/pulsar/pull/6422

- [Function] Support system environment variables in function config (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6348
    
- [Security] Support BouncyCastle FIPS provider (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6588
    
### Notable Bug Fix

- [Schema][Function] Fix Avro schema decode error in functions (Release: 2.5.1, 2.6.0).

    https://github.com/apache/pulsar/pull/6662
    
- [Schema] Parse long field in GenricJsonRecord (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6622

### Ecosystem

- [Pulsar.Client] Pulsar.Client 0.18.0 is released with TLS authentication support.

    https://t.co/QjxquJ7nqI?amp=1
    
- [Pulsar.Client] Pulsar.Client 0.17.0 is released with interceptors support.

    https://www.nuget.org/packages/Pulsar.Client/

### Event / News

- [KoP] StreamNative & OVHcloud open sourced Kafka-on-Pulsar (KoP).

    - Blog: https://streamnative.io/blog/tech/2020-03-24-bring-native-kafka-protocol-support-to-apache-pulsar/

    - Webinar Video: https://www.youtube.com/watch?v=gL6hzRtij8M    

- TGIP (TGI Pulsar) - a weekly live video streaming about Pulsar and its ecosystem.

    - 002: Kubernetes deployment - https://www.youtube.com/watch?v=wGgEx1M17O0

    - 003: Secure a Pulsar cluster with TLS - https://www.youtube.com/watch?v=aP31A-ntHLA
    
    - 004: Deep dive into authentication and authorization - https://www.youtube.com/watch?v=sTISVpyq73o

### Blog / Article

- Why we moved from Apache Kafka to Apache Pulsar (by StreamSQL)

    https://streamsql.io/blog/from-apache-kafka-to-apache-pulsar
    
- Will Apache Pulsar eventually kill Apache Kafka? (by Tarun Manrai)

    https://medium.com/@manrai.tarun/will-apache-pulsar-eventually-kill-apache-kafka-853be9c0ce13
    
- Apache Pulsar outperforms Apache Kafka by 2.5x on OpenMessaging benchmark (by Tarun Manrai)

    https://medium.com/@manrai.tarun/apache-pulsar-outperforms-apache-kafka-by-2-5x-on-openmessaging-benchmark-4838c14a541f
