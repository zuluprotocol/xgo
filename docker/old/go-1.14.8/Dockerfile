# Go cross compiler (xgo): Go 1.14.8
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11408

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.8.linux-amd64.tar.gz    && \
  export ROOT_DIST_SHA=5504e077a29d0bd6649ca7b66e317f1a4b264e960f74115d6f0f405c49a8e738 && \
  \
  $BOOTSTRAP_PURE
