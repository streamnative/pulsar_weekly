---
title: "2020-02-28-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2020-02-15 ~ 2020-02-28"
date: 2020-02-15 ~ 2020-02-28
description: "This is the Pulsar community weekly update for 2020-02-15 ~ 2020-02-28, with updates on improving ZooKeeper session expiry handling, supporting message acknowledgment at the batch index level, release 2.5.1 and many features and bug fixes."
id: "2020-02-28-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2020-02-15 ~ 2020-02-28

This is the Pulsar community weekly update for 2020-02-15 ~ 2020-02-28, with updates on improving ZooKeeper session expiry handling, supporting message acknowledgment at the batch index level, release 2.5.1 and many features and bug fixes.

### Development

- [PIP-57] The discussion of improving Broker's ZooKeeper session expiry handling logic.

    https://lists.apache.org/thread.html/r1f0de583a2d02f9aeff0cadc2bab0fcfb41bf092cfdc7ff4cc9ed1bc%40%3Cdev.pulsar.apache.org%3E
    https://github.com/apache/pulsar/wiki/PIP-57%3A-Improve-Broker%27s-Zookeeper-Session-Timeout-Handling
    
- [PIP-54] Support message acknowledgment at the batch index level.

    https://lists.apache.org/thread.html/rdcc306653be6ac6d910e7302096ddae8e1a9e563df20cf6ca73085de%40%3Cdev.pulsar.apache.org%3E
    https://github.com/apache/pulsar/wiki/PIP-54:-Support-acknowledgment-at-batch-index-level

- [PIP-58] Allow configuring a retry topic for consumers to customize retry delay when using dead letter topic feature.

    https://lists.apache.org/thread.html/r5ab7533b6461f29b8ff18e4c51e058226a1b3081fddc5649b234b7fc%40%3Cdev.pulsar.apache.org%3E
    https://github.com/apache/pulsar/wiki/PIP-58-%3A-Support-Consumers--Set-Custom-Retry-Delay
    
- [Release 2.5.1] Guangning started the discussion of releasing 2.5.1 version.

    https://lists.apache.org/thread.html/rfb8dcda87b8fefb474d1c06d97ab53d608f8364f0f6f65f47dd7025c%40%3Cdev.pulsar.apache.org%3E

### Notable Feature
    
- [Broker] Introduce maxMessagePublishBufferSizeInMB configuration to avoid broker OOM (Release: 2.6.0).
    
    https://github.com/apache/pulsar/pull/6178

- [CLI] Support `unload` all partitions of a partitioned topic (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6187

- [Admin] Enable get precise backlog and backlog without delayed messages (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6310
    
- [SQL] KeyValue schema support for pulsar sql (Release: 2.6.0).

    https://github.com/apache/pulsar/pull/6325

### Notable Bug Fix

- [Broker] Avoid getting partition metadata while the topic name is a partition name (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6339
    
- [Broker] Creating a topic does not wait for creating cursor of replicators (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6364
    
- [Broker] Seek to the first one >= timestamp (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6393
    
- [Broker] Start reader inside batch result in reading first message in batch (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6345
    
- [Broker] Consumers received duplicated deplayed messages upon restart.

    https://github.com/apache/pulsar/pull/6404
    
- [Client][Java] Stop shade snappy-java in pulsar-client-shaded (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6375
    
- [Client] Fix publish buffer limit does not take effect (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6431
    
- [Schema] Fix the problem with parsing of an Avro schema related to shading in pulsar-client.

    https://github.com/apache/pulsar/pull/6406
    
- [Proxy][Security] Fix the bug of authenticationData isn't initialized (Release: 2.6.0, 2.5.1).

    https://github.com/apache/pulsar/pull/6440
    

### Event / News

- [Summit] Pre-registration for Pulsar Summit 2020 is open. Welcome to join the first-ever Pulsar conference with 20+ in-depth technical talks from event streaming experts and connect to the messaging and streaming community.

    https://pulsar-summit.org/

