FROM ghcr.io/home-assistant/base-python:3.15-alpine3.22

ARG BUILD_ARCH
ARG UNIVERSAL_SILABS_FLASHER=0.0.13

RUN \
    set -x \
    && apk add --no-cache \
        py3-pip \
        python3 \
    && pip3 install \
        --no-cache-dir \
        --prefer-binary \
        --find-links "https://wheels.home-assistant.io/musllinux/${BUILD_ARCH}/" \
        universal-silabs-flasher=="${UNIVERSAL_SILABS_FLASHER}"

COPY rootfs /

# use s6-overlay as init system
WORKDIR /
ENTRYPOINT ["/init"]
