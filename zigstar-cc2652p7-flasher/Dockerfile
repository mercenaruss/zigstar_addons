FROM ghcr.io/home-assistant/base-python:3.13-alpine3.22

# cc1352-flasher is pinned to a specific commit for reproducible builds.
RUN \
    set -x \
    && apk add --no-cache \
        py3-pip \
        python3 \
    && apk add --no-cache --virtual .build-deps git \
    && pip3 uninstall -y setuptools \
    && pip3 install --no-cache-dir gpiod==1.5.4 intelhex==2.3.0 pyserial==3.5b0 python_magic==0.4.27 scripttest==1.3 setuptools==52.0.0 \
    && python3 -m pip install --no-cache-dir git+https://github.com/tube0013/cc1352-flasher.git@fd65db12968f73b6946a8385388f4f5647b74653 \
    && apk del .build-deps


COPY rootfs /

# use s6-overlay as init system
WORKDIR /
ENTRYPOINT ["/init"]
