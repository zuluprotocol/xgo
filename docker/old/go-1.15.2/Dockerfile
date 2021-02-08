# Go cross compiler (xgo): Go 1.15.2
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11502

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.2.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=b49fda1ca29a1946d6bb2a5a6982cf07ccd2aba849289508ee0f9918f6bb4552 && \
  \
  $BOOTSTRAP_PURE
