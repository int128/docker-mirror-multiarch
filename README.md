# docker-mirror-multiarch [![mirror](https://github.com/int128/docker-mirror-multiarch/actions/workflows/mirror.yaml/badge.svg)](https://github.com/int128/docker-mirror-multiarch/actions/workflows/mirror.yaml)

This repository shows how to mirror a multi-architecture Docker image.

## Problem to solve

We cannot mirror a multi-architecture image by `docker pull && docker push`.
It copies only single architecture image.

## How to solve

See [mirror workflow](.github/workflows/mirror.yaml).

This is based on https://stackoverflow.com/questions/68567983/how-to-copy-multi-arch-docker-images-to-a-different-container-registry and using [regclient](https://github.com/regclient/regclient).
