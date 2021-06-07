# Go cross compiler (xgo): Go 1.16.4
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11604

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.16.4.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=7154e88f5a8047aad4b80ebace58a059e36e7e2e4eb3b383127a28c711b4ff59 && \
  \
  $BOOTSTRAP_PURE
