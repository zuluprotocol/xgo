# Go cross compiler (xgo): Go 1.15.1
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11501

RUN sed --in-place -e '/darwin.*386/d' /bootstrap_pure.sh

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.15.1.linux-amd64.tar.gz && \
  export ROOT_DIST_SHA=70ac0dbf60a8ee9236f337ed0daa7a4c3b98f6186d4497826f68e97c0c0413f6 && \
  \
  $BOOTSTRAP_PURE
