# Go cross compiler (xgo): Go 1.15.10
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11510

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.10.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=4aa1267517df32f2bf1cc3d55dfc27d0c6b2c2b0989449c96dd19273ccca051d && \
  \
  $BOOTSTRAP_PURE
