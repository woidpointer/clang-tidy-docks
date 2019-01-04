FROM ubuntu:16.04

RUN apt-get update
RUN apt-get install -y xz-utils build-essential curl cmake
RUN curl -SL http://releases.llvm.org/7.0.0/clang+llvm-7.0.0-x86_64-linux-gnu-ubuntu-16.04.tar.xz | \
  tar -xJC . 
RUN mv clang+llvm-7.0.0-x86_64-linux-gnu-ubuntu-16.04 /opt/clang_7.0.0

ENV PATH /opt/clang_7.0.0/bin:$PATH
ENV LD_LIBRARY_PATH /opt/clang_7.0.0/lib:$LD_LIBRARY_PATH

ENV CC /opt/clang_7.0.0/bin/clang 
ENV CXX /opt/clang_7.0.0/bin/clang++





