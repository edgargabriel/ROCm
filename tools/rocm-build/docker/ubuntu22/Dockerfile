FROM ubuntu:jammy as builder
COPY packages /tmp/packages
COPY local-pin-600 /tmp/local-pin-600
COPY install-prerequisities.sh /tmp/install-prerequisities.sh
RUN chmod +x /tmp/install-prerequisities.sh
ENV KBUILD_PKG_ROOTCMD=
ENV RPP_DEPS_LOCATION=/usr/local/rpp-deps
RUN  /tmp/install-prerequisities.sh
WORKDIR /src
