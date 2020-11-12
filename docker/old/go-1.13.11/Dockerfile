# Go cross compiler (xgo): Go 1.13.11
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11311

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.13.11.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=a4d71ca9e02923fa96669a4b5faf78ee8331b18e7209b09dd87fe763b4838ada && \
  \
  $BOOTSTRAP_PURE
