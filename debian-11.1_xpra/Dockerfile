FROM docker.io/pizzafactory0contorno/piatto-quadrato:debian-11.1_xpra@sha256:affadf873973a3eaff43ef64351048adba4bfedabe9eaaaf6e9acac3b260ed38

USER root
RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y \
      build-essential gdb libtool autotools-dev automake pkg-config bsdmainutils python3 bear \
      libssl-dev libevent-dev libboost-system-dev libboost-filesystem-dev libboost-test-dev libboost-thread-dev \
      libminiupnpc-dev \
      libzmq3-dev \
      libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler \
      libdb-dev libdb++-dev \
      libqrencode-dev && \
    apt-get clean && rm -rf /var/lib/apt/lists/*
USER user
