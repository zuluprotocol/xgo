# Go cross compiler (xgo): Go 1.14.15
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11415

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.15.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=c64a57b374a81f7cf1408d2c410a28c6f142414f1ffa9d1062de1d653b0ae0d6 && \
  \
  $BOOTSTRAP_PURE
