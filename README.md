DevOpen Docker Repo
===================

This repository contains Dockerfile of DevOpen IDE for Docker's automated build published to the public Docker Hub Registry.

# Base Docker Image

[kdelfour/supervisor-docker](https://registry.hub.docker.com/u/kdelfour/supervisor-docker/)

# Installation

## Install Docker

Download automated build from public Docker Hub Registry: docker pull fno2010/devopen-headless

(alternatively, you can build an image from Dockerfile: docker build -t="fno2010/devopen-headless" github.com/fno2010/devopen-docker)

## Quick Start

Start a docker instance:

    ./run.sh

## Build and run with custom config directory

Get the latest version from github

    git clone https://github.com/fno2010/devopen-docker
    cd devopen-docker/
    git submodule update --init --recursive

Build it

    sudo ./build.sh

And run

    sudo ./run.sh

It will create a directory named `workspace` under the current path and mount it as the cloud9 workspace.

Enjoy !!

## Acknowledgement

This repo is forked from [kdelfour/cloud9-docker](https://github.com/kdelfour/cloud9-docker).
