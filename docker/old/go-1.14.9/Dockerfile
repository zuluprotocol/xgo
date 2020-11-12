# Go cross compiler (xgo): Go 1.14.9
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11409

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.9.linux-amd64.tar.gz    && \
  export ROOT_DIST_SHA=f0d26ff572c72c9823ae752d3c81819a81a60c753201f51f89637482531c110a && \
  \
  $BOOTSTRAP_PURE
