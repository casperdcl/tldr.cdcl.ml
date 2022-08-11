---
title: Cloud Demigration
src: https://www.protocol.com/enterprise/ai-machine-learning-cloud-data
categories: [Industry, Programming]
tags: [ai, cloud]
---

Migrating away from clouds back to on-premise could be cheaper & more performant.

- :heavy_check_mark: clouds argue that {% glossary ML %} infrastructure is too expensive & difficult to self-host. Also:
  + easily scale compute & storage
  + experts at efficiently maintaining & upgrading hardware
  + [getting faster][awsblog] & [more secure](https://cloud.google.com/blog/topics/hybrid-cloud/announcing-google-distributed-cloud-edge-and-hosted)
- :stop_sign: cloud cons:
  + real-time cloud inference [still a challenge][awsblog]
  + hybrid (cloud + self-host) may be cheaper, e.g. [co-location data centre](https://www.protocol.com/manuals/new-enterprise/data-centers-hybrid-cloud), especially at scale (millions of dollars compute cost)
    * on-prem compute-heavy training, cloud serving
- on-prem pros (especially for smaller teams):
  + :zap: speed: removes cloud data transfer time
  + :lock: security: no need to trust clouds
  + :100: availability: full control over hardware (not shared)
  + :hocho: cutting-edge: don't need to wait for cloud vendors to buy & make available latest hardware

[awsblog]: https://aws.amazon.com/blogs/machine-learning/machine-learning-at-the-edge-with-aws-outposts-and-amazon-sagemaker
