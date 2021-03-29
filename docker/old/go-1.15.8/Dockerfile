# Go cross compiler (xgo): Go 1.15.8
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11508

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b && \
  \
  $BOOTSTRAP_PURE
