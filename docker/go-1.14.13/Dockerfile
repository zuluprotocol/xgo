# Go cross compiler (xgo): Go 1.14.13
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11413

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.13.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=bfea0c8d7b70c1ad99b0266b321608db57df75820e8f4333efa448a43da01992 && \
  \
  $BOOTSTRAP_PURE
