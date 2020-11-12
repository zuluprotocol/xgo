# Go cross compiler (xgo): Go 1.15
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11500

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602 && \
  \
  $BOOTSTRAP_PURE
