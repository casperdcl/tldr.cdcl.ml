---
title: GenesisCloud GPU instances
src: https://developers.genesiscloud.com
categories: [Programming]
tags: [cloud, product-research]
---

New cloud provider focused on low-cost GPUs. Missing an equivalent of auto-scaling groups (ASGs) though.

- [regions](https://developers.genesiscloud.com/regions): `iceland` or `norway`
- [instances](https://developers.genesiscloud.com/regions): focused on consumer GPUs (RTX 3090, 3080, 3060 Ti, 1080 Ti, RX470)
  + 80 GB local disk, no other options. Can't pay for less storage, and have to use volumes (see below) for more storage
  + max 8 RTX 3090s, 32 vCPU, 192 GB RAM, 80 GB disk
  + [schema](https://developers.genesiscloud.com/instances#instance-schema) is fairly intuitive. `is_protected` seems to be the equivalent of `is not spot`
- [images](https://developers.genesiscloud.com/images): `ubuntu`, `tensorflow`, etc...
- [snapshots](https://developers.genesiscloud.com/snapshots): haven't checked - might be what you get automatically on preemption?
- [volumes](https://developers.genesiscloud.com/volumes): can set size & region
- [ssh-keys](https://developers.genesiscloud.com/ssh-keys)
- [security-groups](https://developers.genesiscloud.com/security-groups)
