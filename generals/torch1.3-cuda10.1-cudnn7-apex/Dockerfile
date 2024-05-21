FROM pytorch/pytorch:1.3-cuda10.1-cudnn7-devel

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install wget build-essential -y

# NVIDIA Apex (https://github.com/NVIDIA/apex?tab=readme-ov-file#linux)
RUN pip install packaging && \
    mkdir /packages && \
    cd /packages && \
    git clone https://github.com/NVIDIA/apex && cd apex && \
    pip install -v --disable-pip-version-check --no-build-isolation --no-cache-dir ./

