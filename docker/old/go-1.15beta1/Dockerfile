# Go cross compiler (xgo): Go 1.15beta1
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 115000001

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15beta1.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=11814b7475680a09720f3de32c66bca135289c8d528b2e1132b0ce56b3d9d6d7 && \
  \
  $BOOTSTRAP_PURE
