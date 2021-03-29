# Go cross compiler (xgo): Go 1.16rc1
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11600001

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.16rc1.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=6a62610f56a04bae8702cd2bd73bfea34645c1b89ded3f0b81a841393b6f1f14 && \
  \
  $BOOTSTRAP_PURE
