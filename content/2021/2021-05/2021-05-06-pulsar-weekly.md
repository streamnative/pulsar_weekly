---
title: "2021-05-06-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-04-26 ~ 2021-05-02"
date: 2021-04-26 ~ 2021-05-02
description: "This is the Pulsar community weekly update for 2021-04-26 ~ 2021-05-02, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-05-06-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-04-26 ~ 2021-05-02

This is the Pulsar community weekly update for 2021-04-26 ~ 2021-05-02, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

- [C Client] Fix the issue that the C++ client cannot be built on Windows Operation System (OS).

  https://github.com/apache/pulsar/pull/10363 ([@BewareMyPower](https://github.com/BewareMyPower))
  
- [Broker] Support setting, getting, and removing the property value for a given key on a namespace.

  https://github.com/apache/pulsar/pull/10015 ([@codelipenghui](https://github.com/codelipenghui))
  
### Development

- [PIP-45] Implement load manager locks using coordination service.

  https://github.com/apache/pulsar/pull/10391 ([@merlimat](https://github.com/merlimat))

### Notable Feature

- [Enhancement] Support automatically revalidating resource locks after a metadata session is re-established.

  https://github.com/apache/pulsar/pull/10351 ([@merlimat](https://github.com/merlimat))

- [Transaction] Optimize low watermark for transaction logs.

  https://github.com/apache/pulsar/pull/10422 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Support array-type role claims in JWT authentication.

  https://github.com/apache/pulsar/pull/10375 ([@RobertIndie](https://github.com/RobertIndie))

- [Consumer] Add debug logs when the consumer fails to send permits to the Pulsar broker.

  https://github.com/apache/pulsar/pull/10166 ([@devinbost](https://github.com/devinbost))

- [Broker] Make `LocalPolicies` immutable to avoid concurrent inconsistent modification.

  https://github.com/apache/pulsar/pull/9598 ([@WJL3333](https://github.com/WJL3333))

- [Broker] Improve the `max-pending-bytes` mechanism for the Pulsar broker.

  https://github.com/apache/pulsar/pull/7406 ([@merlimat](https://github.com/merlimat))

- [Tests] Improve the integration test logging to improve readability and efficiency.

  https://github.com/apache/pulsar/pull/10320 ([@lhotari](https://github.com/lhotari))

- [Tests] Re-create keystores used in TLS tests with RSA algorithm and SHA256 to support JDK 11 and TLS 1.3.

  https://github.com/apache/pulsar/pull/10336 ([@lhotari](https://github.com/lhotari))

- [Pulsar SQL] Do not return non-persistent topics when listing tables through Pulsar SQL.

  https://github.com/apache/pulsar/pull/10368 ([@codelipenghui](https://github.com/codelipenghui))

- [Build] Skip tests when only documentation changes are involved for building C++ clients on Windows.

  https://github.com/apache/pulsar/pull/10376 ([@lhotari](https://github.com/lhotari))

- [Auth] Optimize locks in `AuthenticationAthenz`.

  https://github.com/apache/pulsar/pull/10381 ([@massakam](https://github.com/massakam))

- [Build] Add the CI test to verify that the C++ client could be built on the Windows OS.

  https://github.com/apache/pulsar/pull/10387 ([@BewareMyPower](https://github.com/BewareMyPower))
  
- [Functions] Support customized Pulsar Function logs.

  https://github.com/apache/pulsar/pull/10389 ([@devinbost](https://github.com/devinbost))
  
- [Consumer] Adjust logs for locating problem and formatting codes.

  https://github.com/apache/pulsar/pull/10392 ([@linlinnn](https://github.com/linlinnn))

- [Bookie] Fallback to `PULSAR_EXTRA_OPTS` if `BOOKIE_EXTRA_OPTS` is not defined.

  https://github.com/apache/pulsar/pull/10397 ([@lhotari](https://github.com/lhotari))

- [Broker] Prevent carrying the state of `PositionImplRecyclable` when instances are being recycled.

  https://github.com/apache/pulsar/pull/10404 ([@lhotari](https://github.com/lhotari))

- [Java Client] Reset the state before recycling the `OpSendMsg` instance.

  https://github.com/apache/pulsar/pull/10405 ([@lhotari](https://github.com/lhotari))

- [Broker] Make `Persistent*DispatcherMultipleConsumers.readMoreEntries` synchronized.

  https://github.com/apache/pulsar/pull/10413 ([@lhotari](https://github.com/lhotari))

- [C++ Client] Add the `is_connected` method to the C++ API.

  https://github.com/apache/pulsar/pull/10415 ([@k2la](https://github.com/k2la))

- [Connectors] Use `ObjectMapper` instead of `Gson` to parse the source or sink configuration.

  https://github.com/apache/pulsar/pull/10441 ([@abhilashmandaliya](https://github.com/abhilashmandaliya))

### Notable Bug Fix

- [Broker] Fix `ConcurrentModificationException` when attempting to update the local broker data.

  https://github.com/apache/pulsar/pull/10347 ([@315157973](https://github.com/315157973))
  
- [Tests] Fix the `testOffloadV2` flaky test.

  https://github.com/apache/pulsar/pull/10350 ([@315157973](https://github.com/315157973))

- [Transaction] Fix the transaction timeout tracker expired issue.

  https://github.com/apache/pulsar/pull/10366 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Fix the schema type check issue when using the `ALWAYS_COMPATIBLE ` strategy.

  https://github.com/apache/pulsar/pull/10367 ([@codelipenghui](https://github.com/codelipenghui))

- [Tests] Fix the `TestDefaultMessageFormatter` flaky test.

  https://github.com/apache/pulsar/pull/10379 ([@lhotari](https://github.com/lhotari))

- [Broker] Fix the schema ledger deletion issue when deleting topics with the deleted schema.

  https://github.com/apache/pulsar/pull/10383 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the primitive schema upload issue for `ALWAYS_COMPATIBLE` strategy.

  https://github.com/apache/pulsar/pull/10386 ([@codelipenghui](https://github.com/codelipenghui))

- [Broker] Fix the issue in reusing `EntryBatchIndexesAcks` instances.

  https://github.com/apache/pulsar/pull/10400 ([@lhotari](https://github.com/lhotari))

- [Transaction] Fix the issue that the transaction buffer client channel is not active.

  https://github.com/apache/pulsar/pull/10407 ([@congbobo184](https://github.com/congbobo184))

- [Transaction] Fix the issue that the transaction buffer handler does not release semaphore.

  https://github.com/apache/pulsar/pull/10412 ([@congbobo184](https://github.com/congbobo184))

- [Connectors] Fix null error messages in `onFailure` exception for the Kinesis sink connector.

  https://github.com/apache/pulsar/pull/10416 ([@RobertIndie](https://github.com/RobertIndie))

- [Connectors] Fix the issue that the Kinesis sink connector fails to retry to send messages.

  https://github.com/apache/pulsar/pull/10420 ([@RobertIndie](https://github.com/RobertIndie))

- [Transaction] Fix the transaction buffer handler synchronization issue.

  https://github.com/apache/pulsar/pull/10424 ([@congbobo184](https://github.com/congbobo184))

- [Broker] Fix the issue that no error log or exception is generated when topics are being loaded while the replicator fails to be created.

  https://github.com/apache/pulsar/pull/10432 ([@rdhabalia](https://github.com/rdhabalia))

- [Broker] Unblock the stuck thread on update-partition API.

  https://github.com/apache/pulsar/pull/10447 ([@rdhabalia](https://github.com/rdhabalia))
  
- [Build] Fix the `core-modules` profile on JDK11.

  https://github.com/apache/pulsar/pull/10340 ([@lhotari](https://github.com/lhotari))

- [Tests] Fix the issue that the `WebSocketHttpServletRequestWrapperTest` is failed on branch 2.7.

  https://github.com/apache/pulsar/pull/10453 ([@eolivelli](https://github.com/eolivelli))

- [Build] Fix the build error on branch 2.7.

  https://github.com/apache/pulsar/pull/10448 ([@zymap](https://github.com/zymap))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

  - All video recordings are available at [here](https://streamnative.io/resource#tgip).

- [Pulsar Office Hour] Monthly live stream about Pulsar best practices, use cases, and more.

  - 04/30: https://www.youtube.com/watch?v=lREz9eC-pkE

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

  - Europe Edition: Intro to Apache Pulsar EP03

    - 04/29: https://www.youtube.com/watch?v=d_FhP6Nsfm4

- Pulsar Virtual Summit North America 2021

    Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

### Blog / Article

- Function Mesh - Simplify Complex Streaming Jobs in Cloud

  - https://streamnative.io/en/blog/release/2021-05-03-function-mesh-open-source

- Announcing AMQP 1.0 Connector for Apache Pulsar

  - https://streamnative.io/en/blog/tech/2021-04-26-announcing-amqp10-connector-for-apache-pulsar