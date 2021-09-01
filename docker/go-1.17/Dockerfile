# Go cross compiler (xgo): Go 1.17
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11700

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.17.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d && \
  \
  $BOOTSTRAP_PURE
