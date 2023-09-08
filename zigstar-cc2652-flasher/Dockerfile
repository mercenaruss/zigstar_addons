ARG BUILD_FROM
ARG BUILD_ARCH

FROM $BUILD_FROM


RUN \
    set -x \
    && apk add --no-cache \
        py3-pip \
        python3 \
        git \
    && pip3 install git+https://git.beagleboard.org/beagleconnect/cc1352-flasher.git intelhex

COPY rootfs /

# use s6-overlay as init system
WORKDIR /
ENTRYPOINT ["/init"]
