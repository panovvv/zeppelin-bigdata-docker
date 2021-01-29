# Big data playground: Zeppelin

[![Docker Build](https://img.shields.io/docker/cloud/build/panovvv/zeppelin-bigdata.svg)](https://cloud.docker.com/repository/docker/panovvv/zeppelin-bigdata/builds)
[![Docker Pulls](https://img.shields.io/docker/pulls/panovvv/zeppelin-bigdata.svg)](https://hub.docker.com/r/panovvv/zeppelin-bigdata)
[![Docker Stars](https://img.shields.io/docker/stars/panovvv/zeppelin-bigdata.svg)](https://hub.docker.com/r/panovvv/zeppelin-bigdata)

Zeppelin Docker image built on top of Hadoop+Hive+Spark

## Software

* [Zeppelin 0.9.0](https://zeppelin.apache.org/docs/0.9.0/) 

## Usage

Take a look [at this repo](https://github.com/panovvv/bigdata-docker-compose)
to see how I use it as a part of a Docker Compose cluster.

## Maintaining

* Docker file code linting:  `docker run --rm -i hadolint/hadolint < Dockerfile`
* [To trim the fat from Docker image](https://github.com/wagoodman/dive)
