# docker-go-oci8

[![Build Status](https://travis-ci.org/jeanmorais/docker-go-oci8.svg?branch=master)](https://travis-ci.org/jeanmorais/docker-go-oci8)


Dockerfile for building Golang apps with Oracle Instant Client and [mattn/go-oci8](https://github.com/mattn/go-oci8).


The base image is [golang](https://hub.docker.com/_/golang) (default/based on Debian), because `glibc` is required for the build.

## Required

The required files are in [oracle](/oracle) directory.

The packages (`instantclient-sdk-linux` and `instantclient-sdk-linux`) were originally downloaded from the [Oracle Site](https://www.oracle.com/technetwork/topics/linuxx86-64soft-092277.html), and unnecessary files were removed.

## Usage 

```
docker build -t go-oci8 .
```
