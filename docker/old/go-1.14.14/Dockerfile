# Go cross compiler (xgo): Go 1.14.14
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11414

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.14.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=6f1354c9040d65d1622b451f43c324c1e5197aa9242d00c5a117d0e2625f3e0d && \
  \
  $BOOTSTRAP_PURE
