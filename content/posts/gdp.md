+++
title = 'Global Data Plane'
date = 2023-10-22T12:18:39-07:00
draft = false
+++

Today’s exciting new world of data-driven technology, AI, and cyber-physical systems rely on
information from widely disparate sources, combining processing and storage in the cloud with embedded
sensors, actuators, and processing at the edge. This information includes both the inputs and outputs of
computations as well as multi-versioned executables that drive such computations. Edge computing is
essential, since sensors at the edge of the network (e.g., cameras) generate huge volumes of data that is
ideally processed or distilled locally. Further, control loops with sensors, computing, and actuators require
local communication for responsiveness and quality of service (QoS).

Unfortunately, the edge of the network consists of islands of trusted hardware interspersed with a vast sea
of untrusted hardware. Thus, there is a pressing need for connected systems to uniformly verify the integrity
of the information on which they rely and similarly to provide a universal audit-trail for the information that they
produce. Further, privacy must be respected by the infrastructure and relinquished only when necessary.

To address these needs, we propose a fundamental refactoring of the network around cryptographically
hardened bundles of data, called DataCapsules. DataCapsules are the cyberspace equivalent of shipping
containers: uniquely named, secured bundles of information transported over a data-centric “narrow-waist”
infrastructure called the Global Data Plane (GDP). The GDP partitions the network into Trust Domains (TDs)
to allow clients to reason about the trustworthiness of hardware. When combined with trusted computing
enclaves, the GDP enables applications to dynamically partition their functionality between the cloud and
network edge, yielding better QoS, lower latency, and enhanced privacy without risking information integrity
or obscuring its provenance.

## Paper Link(s)

[Towards a Global Data Infrastructure](https://ieeexplore.ieee.org/document/7436637)

[Nitesh Mor's PhD thesis](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2020/EECS-2020-10.html)

[TrustNet](https://grapheo12.in/404)