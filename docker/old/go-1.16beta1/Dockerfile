# Go cross compiler (xgo): Go 1.16beta1
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 116000001

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8 && \
  \
  $BOOTSTRAP_PURE
