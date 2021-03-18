# Docker-Ubuntu 

## About

Dockerfile to build a ubuntu:focal (20.04) base image with a couple of extra packages.  I am leveraging [sameersbn's](https://github.com/sameersbn/docker-ubuntu) image as a starting point, but updating it for  a more recent release of ubuntu.

The image is built on top of the most recently tagged `ubuntu:focal` image and installs the following extra packages:

- `vim.tiny`
- `wget`
- `sudo`
- `net-tools`
- `ca-certificates`
- `unzip`
- `tzdata`

The packages are selected based on the criteria that they are commonly used and that they do not influence the size of the resulting image too much.

Additionally `apt` is configured to **NOT** install `recommended` and `suggested` packages.
