+++
title = 'Paranoid Stateful Lambdas'
date = 2023-11-02T12:11:45-07:00
draft = false
+++

We propose a federated Function-as-a-Service (FaaS) execution model that provides secure and stateful execution in both Cloud and Edge environments. The FaaS workers, called Paranoid Stateful Lambdas (PSLs), collaborate with one another to perform large parallel computations. We exploit cryptographically hardened and mobile bundles of data, called DataCapsules, to provide persistent state for our PSLs, whose execution is protected using hardware-secured TEEs. To make PSLs easy to program and performant, we build the familiar Key-Value Store interface on top of DataCapsules in a way that allows amortization of cryptographic operations. We demonstrate PSLs functioning in an edge environment running on a group of Intel NUCs with SGXv2.

As described, our Secure Concurrency Layer (SCL), provides eventually-consistent semantics over written values using untrusted and unordered multicast. All SCL communication is encrypted, unforgeable, and private. For durability, updates are recorded in replicated DataCapsules, which are append-only cryptographically-hardened blockchain with confidentiality, integrity, and provenance guarantees. Values for inactive keys are stored in a log-structured merge-tree (LSM) in the same DataCapsule. SCL features a variety of communication optimizations, such as an efficient message passing framework that reduces the latency up to 44x from the Intel SGX SDK, and an actor-based cryptographic processing architecture that batches cryptographic operations and increases throughput by 81x.

## Paper Link(s)

[ArXiv link](https://arxiv.org/abs/2210.11703)

[SOSP 2023 Poster](/files/sosp_2023_psl_poster.pdf)
