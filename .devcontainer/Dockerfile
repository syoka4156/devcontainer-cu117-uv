ARG VARIANT="11.7.1-cudnn8-runtime-ubuntu20.04"

FROM nvidia/cuda:${VARIANT}

RUN apt-get update && apt-get install -y \
    curl \
    git \
    && apt-get upgrade -y \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN curl -LsSf https://astral.sh/uv/0.4.6/install.sh | sh 

WORKDIR /workspace
