---
title: "2021-04-19-pulsar-weekly"
displayTitle: "Pulsar Community Weekly Update - 2021-04-12 ~ 2021-04-18"
date: 2021-04-12 ~ 2021-04-18
description: "This is the Pulsar community weekly update for 2021-04-12 ~ 2021-04-18, with updates on Pulsar client, broker, transactions, and so on."
id: "2021-04-19-pulsar-weekly"
---

## [Pulsar Community Weekly Update] 2021-04-12 ~ 2021-04-18

This is the Pulsar community weekly update for 2021-04-12 ~ 2021-04-18, with updates on Pulsar client, broker, transactions, and so on.

### Pulsar Highlight

In `SinkRecord#getSchema`, unwrap the `AutoConsumeSchema` schema to access the actual schema set on the topic. It allows handling topics with the `KeyValue` schema.

by (@[eolivelli](https://github.com/eolivelli))

### Development

- [PIP-82] [Broker] Implement ResourceGroup service, usage-data gathering and quota calculation.

    https://github.com/apache/pulsar/pull/10204 (@[kaushik-develop](https://github.com/kaushik-develop))

### Notable Feature

- [CLI] Expose the `metrics-port-start` local-run configuration to the CLI.

    https://github.com/apache/pulsar/pull/10185 (@[jerrypeng](https://github.com/jerrypeng))

- [Schema Registry] Handle KeyValue with SEPARATED encoding.

    https://github.com/apache/pulsar/pull/10186 (@[eolivelli](https://github.com/eolivelli))
    
- [Tests] Enable test retries for integration tests, shade tests and backwards compatibility tests.

    https://github.com/apache/pulsar/pull/10191 (@[lhotari](https://github.com/lhotari))
    
- [CI] Move flaky tests that often fail to quarantine the test group.

    https://github.com/apache/pulsar/pull/10148 (@[lhotari](https://github.com/lhotari))
    
- [Tests] Add `TestNG` listeners to mitigate resource cleanup issues.

    https://github.com/apache/pulsar/pull/10195 (@[lhotari](https://github.com/lhotari))
    
- [CI] Add the current IP address, long hostname and short hostname to `/etc/hosts`.

    https://github.com/apache/pulsar/pull/10233 (@[lhotari](https://github.com/lhotari))
    
- [CI] Tune GitHub Runner VM options to increase working RAM and improve performance.

    https://github.com/apache/pulsar/pull/10239 (@[lhotari](https://github.com/lhotari))
    
- [Admin] Support starting from the separate `MessageId` for each topic or partition.

    https://github.com/apache/pulsar/pull/10033 (@[315157973](https://github.com/315157973))
    
- [Transactions] Support transactions in Pulsar standalone mode.

    https://github.com/apache/pulsar/pull/10238 (@[congbobo184](https://github.com/congbobo184))
    
- [Tests] Cleanup `PulsarClient` instances.

    https://github.com/apache/pulsar/pull/10197 (@[lhotari](https://github.com/lhotari))
    
- [WebSocket Client] Remove the `Bearer` prefix requirement for the token parameter value of the WebSocket URL.

    https://github.com/apache/pulsar/pull/10187 (@[gaoran10](https://github.com/gaoran10))
    
- [Broker] Add `preciseTopicPublishRateLimiterEnable` to the `broker.conf` file

    https://github.com/apache/pulsar/pull/10216 (@[lhotari](https://github.com/lhotari))
    
- [Tests] In general, the broker is shut down gracefully. However, when the `brokerShutdownTimeoutMs` is reached, the broker should be shut down forcefully.

    https://github.com/apache/pulsar/pull/10199 (@[lhotari](https://github.com/lhotari))
    
- [Tests] Speed up execution of flaky test group and improve the test coverage of test listeners.

    https://github.com/apache/pulsar/pull/10249 (@[lhotari](https://github.com/lhotari))
    
- [Schema Registry] Unwrap the internal `AutoConsumeSchema` to handle topics with the `KeyValue` schema.

    https://github.com/apache/pulsar/pull/10211 (@[eolivelli](https://github.com/eolivelli))

### Notable Bug Fix

- [Tests] Fix Prometheus metrics parsing for "+Inf" in `PrometheusMetricsTest` and Pulsar Function tests.

    https://github.com/apache/pulsar/pull/10193 (@[lhotari](https://github.com/lhotari))
    
- [Client] Fix memory leak issues.

    https://github.com/apache/pulsar/pull/10028 (@[abhilashmandaliya](https://github.com/abhilashmandaliya))
    
    
- [Build] Fix the warning about `parent.relativePath` in `buildtools/pom.xml` file.

    https://github.com/apache/pulsar/pull/10194 (@[lhotari](https://github.com/lhotari))
    
- [Tests] Un-register `JettyStatisticsCollector` to fix memory leak when shutting down the broker.

    https://github.com/apache/pulsar/pull/10192 (@[lhotari](https://github.com/lhotari))
    
- [Tests] Fix some `ExecutorService` leaks.

    https://github.com/apache/pulsar/pull/10198 (@[lhotari](https://github.com/lhotari))
    
- [Broker] Update the authentication data when an authentication refresh happens.

    https://github.com/apache/pulsar/pull/10203 (@[kaushik-develop](https://github.com/kaushik-develop))
    
- [Broker] Close namespace clients when `PulsarService` is closed.

    https://github.com/apache/pulsar/pull/10196 (@[lhotari](https://github.com/lhotari))
    
- [Enhancement] Update `chuckedMessageRate` to `chunkedMessageRate` without breaking the public API.

    https://github.com/apache/pulsar/pull/10223 (@[michaeljmarshall](https://github.com/michaeljmarshall))

- [Security] Upgrade the JUnit version to 4.13.1 to resolve CVE-2020-15250 and fix the test dependency leak.

    https://github.com/apache/pulsar/pull/10147 (@[lhotari](https://github.com/lhotari))
    
- [ManagedLedger] Fix the update logic of the entry cache size to prevent it from getting a negative value.

    https://github.com/apache/pulsar/pull/10225 (@[MarvinCai](https://github.com/MarvinCai))
    
- [CLI] Fix NPE in `CmdTopics`.

    https://github.com/apache/pulsar/pull/10178 (@[linlinnn](https://github.com/linlinnn))
    
- [Tests] Fix the TCP port conflicts in tests.

    https://github.com/apache/pulsar/pull/10209 (@[lhotari](https://github.com/lhotari))
    
- [Tests] Fix test retries for shade tests and backwards compatibility tests.

    https://github.com/apache/pulsar/pull/10207 (@[lhotari](https://github.com/lhotari))
    
- [Broker] Remove unnecessary bundle listener triggers when looking up topics.

    https://github.com/apache/pulsar/pull/10126 (@[hangc0276](https://github.com/hangc0276))
    
- [Broker] Fix replicated subscriptions related `LightProto` issues.

    https://github.com/apache/pulsar/pull/10247 (@[lhotari](https://github.com/lhotari))
    
- [C++] Fix use-after-free undefined behavior due to object lifetime problem.

    https://github.com/apache/pulsar/pull/10220 (@[oversearch](https://github.com/oversearch))
    
- [Broker] Fix the compilation failure in the master branch.

    https://github.com/apache/pulsar/pull/10250 (@[lhotari](https://github.com/lhotari))
    
- [Security] Upgrade jclouds to 2.3.0 to fix security vulnerabilities.

    https://github.com/apache/pulsar/pull/10149 (@[lhotari](https://github.com/lhotari))
    
- [Client][Proxy] Create a copy of response messages before passing them to other threads through `CompletableFuture`.

    https://github.com/apache/pulsar/pull/10215 (@[lhotari](https://github.com/lhotari))

### Event / News

- [TGIP] Weekly live stream about Pulsar and its ecosystem.

    - 021: April Updates on Apache Pulsar
  
        - https://www.youtube.com/watch?v=YH9CidHinCQ

- [Intro to Apache Pulsar 101] Monthly live stream about Pulsar, including concepts, architecture, and design.

    - All video recordings are available at [here](https://streamnative.io/en/resource#intro-to-apache-pulsar-101).

- Apache Pulsar Hackathon

    Sign-up: https://www.eventbrite.com/e/apache-pulsar-hackathon-2021-tickets-143906003731

- Pulsar Virtual Summit North America 2021

    Sign-up: https://hopin.com/events/pulsar-summit-north-america-2021

### Blog / Article

- Call for Beta Users: Function Mesh Now Available for Pulsar Functions

    - https://streamnative.io/en/blog/release/2021-04-05-call-for-beta-users-function-mesh-now-available-for-pulsar-functions

