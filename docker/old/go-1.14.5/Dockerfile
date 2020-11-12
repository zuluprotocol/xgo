# Go cross compiler (xgo): Go 1.14.5
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11405

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.5.linux-amd64.tar.gz    && \
  export ROOT_DIST_SHA=82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b && \
  \
  $BOOTSTRAP_PURE
