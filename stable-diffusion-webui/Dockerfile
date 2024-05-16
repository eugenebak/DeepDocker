FROM nvcr.io/nvidia/cuda:11.6.1-devel-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive

WORKDIR /workspace

RUN apt-get update && apt-get install vim -y

# Dependencies for Stable diffusion WebUI (https://github.com/AUTOMATIC1111/stable-diffusion-webui?tab=readme-ov-file#automatic-installation-on-linux)
RUN apt install wget git python3 python3-venv libgl1 libglib2.0-0 -y

RUN wget -q https://raw.githubusercontent.com/AUTOMATIC1111/stable-diffusion-webui/master/webui.sh
