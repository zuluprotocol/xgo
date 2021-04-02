# Go cross compiler (xgo): Go 1.16.2
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11602

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8 && \
  \
  $BOOTSTRAP_PURE
