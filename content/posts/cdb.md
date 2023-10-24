+++
title = 'CapsuleDB'
date = 2023-10-23T12:10:07-07:00
draft = false
+++

Secure stateful computation in the edge environment is a difficult problem to solve due to limitations on storage capacity and compute hardware.
With the advent of Internet-of-Things, the need for confidential computing and secure storage on top of untrusted hardware is increasing.

In this premise, we present CapsuleDB, a key-value store
for edge devices that provides confidentiality through trusted
execution environments (TEEs). CapsuleDB stores data in
cryptographically hardened containers called DataCapsules,
which allow for maintaining data integrity and provenance
even on top of remote untrusted storage systems. Instead of
porting existing key-value stores into a TEE, we build the
application from scratch, providing several optimizations in
caching, compaction and indexing to overcome the memory
limitations of a TEE. We find that even with all TEE and
cryptographic overheads, CapsuleDB is only 1.9-3.1x slower
than RocksDB, a state-of-the-art unsecure key-value store,
for moderate workload sizes.

## Paper Link(s)

[CapsuleDB v1](https://digicoll.lib.berkeley.edu/record/269485)

[CapsuleDB v2](https://people.eecs.berkeley.edu/~kubitron/courses/cs262a-F22/projects/reports/project7_report.pdf)

