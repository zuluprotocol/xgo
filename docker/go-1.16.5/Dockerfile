# Go cross compiler (xgo): Go 1.16.5
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo:base

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11605

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.16.5.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061 && \
  \
  $BOOTSTRAP_PURE
