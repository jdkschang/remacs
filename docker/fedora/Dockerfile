FROM fedora:latest

RUN dnf install -y \
    git \
    gcc gcc-c++ \
    kernel-devel \
    make \
    automake \
    ncurses-devel \
    giflib-devel \
    libjpeg-turbo-devel \
    libtiff-devel \
    gtk3-devel \
    libxml2-devel \
    libXpm-devel \
    gnutls-devel \
    clang-devel \
    libXt-devel \
    curl \
    texinfo


ENV PATH "/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin"

RUN curl https://sh.rustup.rs -o rustup.sh && \
    sh rustup.sh \
        --default-host x86_64-unknown-linux-gnu \
        --default-toolchain nightly-2020-04-07 -y && \
    rustup default nightly-2020-04-07

