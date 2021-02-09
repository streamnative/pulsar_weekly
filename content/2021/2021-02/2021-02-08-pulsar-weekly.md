---
title: "2021-02-08-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-02-01 ~ 2021-02-07"
date: 2021-02-01 ~ 2021-02-07
description: "This is the Pulsar community weekly update for 2021-02-01 ~ 2021-02-07, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on."
id: "2021-02-08-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-02-01 ~ 2021-02-07

This is the Pulsar community weekly update for 2021-02-01 ~ 2021-02-07, with updates on Pulsar client, broker, Functions, transactions, authentication, and so on.

### Pulsar Highlight

Fix the batch index acknowledgement persistent issue. Currently, the `batchDeletedIndexInfoBuilder` is reused for generating the batch index acknowledgement data, but the deletion setting is not cleared before adding the new deleting setting.

by (@[codelipenghui](https://github.com/codelipenghui))

### Development

- [SQL] [PIP-71] Pulsar SQL migrate SchemaHandle to the Presto decoder.

    https://github.com/apache/pulsar/pull/8422 (@[hnail](https://github.com/hnail))

- [Broker] [PIP-45] Implement the distributed ID generator using the coordination service.

    https://github.com/apache/pulsar/pull/9274 (@[merlimat](https://github.com/merlimat))

- [Metadata] [PIP-45] Add session events to metadata store.

    https://github.com/apache/pulsar/pull/9273 (@[merlimat](https://github.com/merlimat))

### Notable Feature

- [Client] Add default implementation of `CryptoKeyReader`.

    https://github.com/apache/pulsar/pull/9379 (@[massakam](https://github.com/massakam))

- [BookKeeper] Support configuring the BookKeeper `Opportunistic Striping` feature.

    https://github.com/apache/pulsar/pull/9232 (@[eolivelli](https://github.com/eolivelli))

- [Admin] Support getting the applied policy for `MaxConsumers`.

    https://github.com/apache/pulsar/pull/9296 (@[315157973](https://github.com/315157973))

- [Tiered Storage] Allow to refresh the AWS credentials.

    https://github.com/apache/pulsar/pull/9387 (@[addisonj](https://github.com/addisonj))

- [Functions] Expose pulsar-admin client through the Functions context.

    https://github.com/apache/pulsar/pull/9246 (@[freeznet](https://github.com/freeznet))

- [Flaky Test] Add acknowledgement timeout setting for `RetryTopicTest#testRetryTopicWithMultiTopic`.

    https://github.com/apache/pulsar/pull/9334 (@[aloyszhang](https://github.com/aloyszhang))

- [Dead Letter Queue] Avoid enabling DLQ in Key_Shared subscription mode.

    https://github.com/apache/pulsar/pull/9163 (@[MarvinCai](https://github.com/MarvinCai))

- [Broker] Add the streaming dispatcher.

    https://github.com/apache/pulsar/pull/9056 (@[MarvinCai](https://github.com/MarvinCai))

- [Broker] Handle bad-version in metadata-store if the broker updates the ZooKeeper metadata from the ZooKeeper client.

    https://github.com/apache/pulsar/pull/9412 (@[rdhabalia](https://github.com/rdhabalia))

- [Broker] Add alerts for expired/expiring tokens.

    https://github.com/apache/pulsar/pull/9321 (@[RobertIndie](https://github.com/RobertIndie))

- [Test] Add the test for creating producers for non-persistent replicated topics.

    https://github.com/apache/pulsar/pull/9322 (@[congbobo184](https://github.com/congbobo184))

- [Functions] Support setting the memory limit for the Pulsar client used in the `ThreadRuntime` in Pulsar Functions

    https://github.com/apache/pulsar/pull/9320 (@[jerrypeng](https://github.com/jerrypeng))

- [Functions] Optimize the built-in source/sink startup process by eliminating the redundant NAR unpacking and checksum calculation.

    https://github.com/apache/pulsar/pull/9413 (@[jerrypeng](https://github.com/jerrypeng))

- [Admin] Support schema REST API for V1 topics.

    https://github.com/apache/pulsar/pull/9218 (@[rdhabalia](https://github.com/rdhabalia))

- [Functions] Enhance the Kubernetes manifest customizer with default options.

    https://github.com/apache/pulsar/pull/9445 (@[freeznet](https://github.com/freeznet))

- [Managed Ledger] Support configuring the `ManagedLedger` storage.

    https://github.com/apache/pulsar/pull/9397 (@[sijie](https://github.com/sijie))

- [Admin] Ensure that the admin operations on Statestore are not blocked.

    https://github.com/apache/pulsar/pull/9348 ([@pkumar-singh](https://github.com/pkumar-singh))

- [C++] Remove the Boost::System runtime dependency.

    https://github.com/apache/pulsar/pull/9498 (@[merlimat](https://github.com/merlimat))

- [CLI] Update the `-cluster` parameter in t`he delete-cluster-metadata` command to `--cluster`.

    https://github.com/apache/pulsar/pull/9487 (@[yangl](https://github.com/yangl))

- [Topic Policy] Support getting the applied policy for retention.

    https://github.com/apache/pulsar/pull/9362 (@[315157973](https://github.com/315157973))

- [Topic Policy] Support getting the applied policy for the offloader.

    https://github.com/apache/pulsar/pull/9505 (@[315157973](https://github.com/315157973))

### Notable Bug Fix

- [Flaky Test] Fix the `MessagePublishBufferThrottleTest` Flaky test.

    https://github.com/apache/pulsar/pull/9376 (@[Renkai](https://github.com/Renkai))

- [Flaky Test] Fix the `TopicReaderTest.testMultiReaderIsAbleToSeekWithTimeOnMiddleOfTopic` Flaky test.

    https://github.com/apache/pulsar/pull/9375 (@[Renkai](https://github.com/Renkai))

- [C++] Fix the issue that pulsar-client-java does not set `replicator_to` into messages when batching is enabled.

    https://github.com/apache/pulsar/pull/9372 (@[k2la](https://github.com/k2la))

- [Admin] Fix the issue that the `backlogQuota` is updated successfully even if there is a check error.

    https://github.com/apache/pulsar/pull/9382 (@[315157973](https://github.com/315157973))

- [Go Functions] Fix the metrics server handler error.

    https://github.com/apache/pulsar/pull/9394 (@[freeznet](https://github.com/freeznet))

- [Broker] Skip clearing delayed messages when dispatching is not initialized.

    https://github.com/apache/pulsar/pull/9378 (@[codelipenghui](https://github.com/codelipenghui))

- [Functions] Fix the issue that the `narExtractionDirectory`  is not set by the `broker.conf` directly.

    https://github.com/apache/pulsar/pull/9319 (@[hangc0276](https://github.com/hangc0276))

- [Client] Compression must be applied during deferred schema preparation and `enableBatching` is enabled.

    https://github.com/apache/pulsar/pull/9396 (@[eolivelli](https://github.com/eolivelli))

- [Broker] Fixed NPE and cache invalidation in the leader election.

    https://github.com/apache/pulsar/pull/9460 (@[merlimat](https://github.com/merlimat))

- [Broker] Fix the partition number does not equal to the expected error.

    https://github.com/apache/pulsar/pull/9446 (@[codelipenghui](https://github.com/codelipenghui))

- [Schema Registry] Fix the `BookkeeperSchemaStorage` NPE.

    https://github.com/apache/pulsar/pull/9264 (@[codelipenghui](https://github.com/codelipenghui))

- [Flaky Test] Fix the ConsumedLedgersTrimTest.testConsumedLedgersTrimNoSubscriptions Flaky test.

    https://github.com/apache/pulsar/pull/9420 (@[315157973](https://github.com/315157973))

- [Flaky Test] Fix the V1_ProducerConsumerTest.testConcurrentConsumerReceive flaky-test.

    https://github.com/apache/pulsar/pull/9435 (@[315157973](https://github.com/315157973))

- [Functions] Fix the issue that functions cannot be created with m-TLS.

    https://github.com/apache/pulsar/pull/9260 (@[sijie](https://github.com/sijie))

- [Broker] Fix the exception that is thrown when getting optional field for PB messages.

    https://github.com/apache/pulsar/pull/9468 (@[aloyszhang](https://github.com/aloyszhang))

- [Broker] Handle the zk-children watch notification.

    https://github.com/apache/pulsar/pull/9473 (@[rdhabalia](https://github.com/rdhabalia))

- [Flaky Test] Fix the LeaderElection Flaky test.

    https://github.com/apache/pulsar/pull/9443 (@[MarvinCai](https://github.com/MarvinCai))

- [Managed Ledger] Fix the batch index acknowledgement persistent issue.

    https://github.com/apache/pulsar/pull/9504 (@[codelipenghui](https://github.com/codelipenghui))

- [Schema Registry] Fix the topic loading failure due to the broken schema ledger.

    https://github.com/apache/pulsar/pull/9212 (@[rdhabalia](https://github.com/rdhabalia))

- [Flaky Test] Fix the TransactionMetaStoreAssignAndFailover Flaky test.

    https://github.com/apache/pulsar/pull/9506 (@[Renkai](https://github.com/Renkai))

- [Client] Fix the issue that the batch version of `acknowledgeAsync` returns a completed future before individual messages are completed.

    https://github.com/apache/pulsar/pull/9383 (@[congbobo184](https://github.com/congbobo184))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 019: Latest Updates On Apache Pulsar
  
        - https://t.co/zXjaokSGKa?amp=1

### Blog / Article

- How to choose Pulsar vs Kafka? -- Jesse Anderson

    - https://developpaper.com/how-to-choose-pulsar-vs-kafka/
