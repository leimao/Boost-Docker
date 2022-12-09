# Boost Docker

## Introduction

The Docker and CMake examples for Boost C++ Library.

## Docker Container

### Set Boost Library Version

```bash
$ BOOST_VERSION=1.80.0
```

### Build Docker Image

```bash
$ docker build -f docker/boost.Dockerfile --build-arg BOOST_VERSION=${BOOST_VERSION} --tag=boost:${BOOST_VERSION} .
```

### Run Docker Container

```bas
$ docker run -it --rm -v $(pwd):/mnt boost:${BOOST_VERSION}
```

## CMake Examples

Follow the [README](/examples/README.md) in the examples.
