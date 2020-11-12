# Go cross compiler (xgo): Go 1.14.11
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM vegaprotocol/xgo-base:latest

MAINTAINER Péter Szilágyi <peterke@gmail.com>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 11411

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.14.11.linux-amd64.tar.gz   && \
  export ROOT_DIST_SHA=ef150041e1af0890ecdd98ebdd6c759096884052a584c09ce50b2b5bb9bab2cd && \
  \
  $BOOTSTRAP_PURE
