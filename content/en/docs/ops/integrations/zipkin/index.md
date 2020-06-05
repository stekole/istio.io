---
title: Zipkin
description: How to integrate with Zipkin.
weight: 30
keywords: [integration,zipkin,tracing]
test: n/a
---

[Zipkin](https://zipkin.io/) is a distributed tracing system. It helps gather timing data needed to troubleshoot latency problems in service architectures. Features include both the collection and lookup of this data.

## Configuration

Consult the [Zipkin documentation](https://zipkin.io/) to get started. No special changes are needed for Zipkin to work with Istio.

Once Zipkin is installed, you will need to point Istio proxies to send traces to the deployment. This can be configured with `--set values.global.tracer.zipkin.address=<zipkin-collector-address>:9411` at installation time. See the [`ProxyConfig.Tracing`](/docs/reference/config/istio.mesh.v1alpha1/#Tracing) for advanced configuration such as TLS settings.

## Usage

For more information on using Zipkin, please refer to the [Zipkin task](/docs/tasks/observability/distributed-tracing/zipkin/).