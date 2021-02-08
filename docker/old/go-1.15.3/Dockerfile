# Go cross compiler (xgo): Go 1.15.3
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11503

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d && \
  \
  $BOOTSTRAP_PURE
