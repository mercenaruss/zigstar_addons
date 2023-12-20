ARG BUILD_FROM
ARG BUILD_ARCH

FROM $BUILD_FROM


RUN \
    set -x \
    && apk add --no-cache \
    py3-pip \
    python3 \
    git \
    && pip3 uninstall -y setuptools \
    && pip3 install gpiod==1.5.4 intelhex==2.3.0 pyserial==3.5b0 python_magic==0.4.27 scripttest==1.3 setuptools==52.0.0 \
    && python3 -m pip install git+https://github.com/mercenaruss/cc1352-flasher.git


COPY rootfs /

# use s6-overlay as init system
WORKDIR /
ENTRYPOINT ["/init"]
