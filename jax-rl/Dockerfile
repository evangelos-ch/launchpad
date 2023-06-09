FROM python:3.10-slim-buster AS py
ARG VERSION=0.4.11

COPY requirements.txt ./
RUN pip install --no-cache-dir --upgrade pip && \
    pip install "jaxlib[cuda11_cudnn86]==${VERSION}" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html && \
    pip install "jax==${VERSION}" && \
    pip install --no-cache-dir -r requirements.txt

# FROM nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu20.04 AS lib

# # install python3-pip
# RUN apt update && apt install python3-pip -y

WORKDIR /usr/src/app

ENTRYPOINT ["python"]
