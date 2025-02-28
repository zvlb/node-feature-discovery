---
title: "Image variants"
layout: default
sort: 1
---

# Image variants
{: .no_toc}

---

NFD offers two variants of the container image. The "minimal" variant is
deployed by default. Released container images are available for
x86_64 and Arm64 architectures.

## Minimal

This is a minimal image based on
[scratch](https://hub.docker.com/_/scratch)
and only supports running statically linked binaries.

For backwards compatibility a container image tag with suffix `-minimal`
(e.g. `{{ site.container_image }}-minimal`) is provided.

## Full

This image is based on [debian:bookworm-slim](https://hub.docker.com/_/debian)
and contains a full Linux system for running shell-based nfd-worker hooks and
doing live debugging and diagnosis of the NFD images.

The container image tag has suffix `-full`
(e.g. `{{ site.container_image }}-full`).
