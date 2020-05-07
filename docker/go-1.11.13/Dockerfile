# Go cross compiler (xgo): Go 1.11.13
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

#FROM karalabe/xgo-base
FROM docker.pkg.github.com/vegaprotocol/xgo/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11113

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.11.13.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=50fe8e13592f8cf22304b9c4adfc11849a2c3d281b1d7e09c924ae24874c6daa && \
  $BOOTSTRAP_PURE
