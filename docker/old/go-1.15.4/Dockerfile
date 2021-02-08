# Go cross compiler (xgo): Go 1.15.4
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11504

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.4.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=eb61005f0b932c93b424a3a4eaa67d72196c79129d9a3ea8578047683e2c80d5 && \
  \
  $BOOTSTRAP_PURE
