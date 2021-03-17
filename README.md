# Docker-Ubuntu 

## About

Dockerfile to build a ubuntu:20.04 baseimage with a couple of extra packages.  I am leveraging [sameersbn's](https://github.com/sameersbn/docker-ubuntu) image as a starting point, but updating it for  a more recent release of ubuntu.

The image is built on top of the most recently tagged `ubuntu:20.04` image and installs the following extra packages:

- `vim.tiny`
- `wget`
- `sudo`
- `net-tools`
- `ca-certificates`
- `unzip`
- 

The packages are selected based on the criteria that they are commonly used and that they do not influence the size of the resulting image too much.

Additionally `apt` is configured to **NOT** install `recommended` and `suggested` packages.
