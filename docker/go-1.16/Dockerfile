# Go cross compiler (xgo): Go 1.16
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11600

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.16.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=013a489ebb3e24ef3d915abe5b94c3286c070dfe0818d5bca8108f1d6e8440d2 && \
  \
  $BOOTSTRAP_PURE
