# Big data playground: Zeppelin

[![Docker Build](https://img.shields.io/docker/cloud/build/panovvv/zeppelin-bigdata.svg)](https://cloud.docker.com/repository/docker/panovvv/zeppelin-bigdata/builds)
[![Docker Pulls](https://img.shields.io/docker/pulls/panovvv/zeppelin-bigdata.svg)](https://hub.docker.com/r/panovvv/zeppelin-bigdata)
[![Docker Stars](https://img.shields.io/docker/stars/panovvv/zeppelin-bigdata.svg)](https://hub.docker.com/r/panovvv/zeppelin-bigdata)

Zeppelin Docker image built on top of Hadoop+Hive+Spark

Take a look [at this repo](https://github.com/panovvv/bigdata-docker-compose)
to see how I use it as a part of a Docker Compose cluster.

## Software

* [Zeppelin 0.8.2](https://zeppelin.apache.org/docs/0.8.2/) 

## Usage

You should dedicate more RAM to Docker than what it had by default
(2Gb on my machine with 16Gb RAM). Otherwise applications (ResourceManager in my case)
will quit sporadically and you'll see messages like this one in logs:
<pre>
current-datetime INFO org.apache.hadoop.util.JvmPauseMonitor: Detected pause in JVM or host machine (eg GC): pause of approximately 1234ms
No GCs detected
</pre>
Increasing memory to 8G solved all those mysterious problems for me.

## Maintaining

* Docker file code linting:  `docker run --rm -i hadolint/hadolint < Dockerfile`
* [To trim the fat from Docker image](https://github.com/wagoodman/dive)
