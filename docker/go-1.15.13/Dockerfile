# Go cross compiler (xgo): Go 1.15.13
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11513

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.13.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=3d3beec5fc66659018e09f40abb7274b10794229ba7c1e8bdb7d8ca77b656a13 && \
  \
  $BOOTSTRAP_PURE
