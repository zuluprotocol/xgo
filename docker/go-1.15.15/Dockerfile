# Go cross compiler (xgo): Go 1.15.15
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11515

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.15.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=0885cf046a9f099e260d98d9ec5d19ea9328f34c8dc4956e1d3cd87daaddb345 && \
  \
  $BOOTSTRAP_PURE
