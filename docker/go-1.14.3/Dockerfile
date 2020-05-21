# Go cross compiler (xgo): Go 1.14.3
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

#FROM karalabe/xgo-base
FROM docker.pkg.github.com/vegaprotocol/xgo/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11403

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.3.linux-amd64.tar.gz    && \
  export ROOT_DIST_SHA=1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226 && \
  \
  $BOOTSTRAP_PURE
