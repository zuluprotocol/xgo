# Go cross compiler (xgo): Go 1.14.10
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11410

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.10.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=66eb6858f375731ba07b0b33f5c813b141a81253e7e74071eec3ae85e9b37098 && \
  \
  $BOOTSTRAP_PURE
