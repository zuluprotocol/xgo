# Go cross compiler (xgo): Go 1.14.4
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11404

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.4.linux-amd64.tar.gz    && \
  export ROOT_DIST_SHA=aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067 && \
  \
  $BOOTSTRAP_PURE
