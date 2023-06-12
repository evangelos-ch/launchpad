FROM python:3.10-slim-buster
LABEL maintainer="me@evangelos.ai"

RUN apt-get update && apt install -y --no-install-recommends git python3-pip

WORKDIR /usr/src/app
COPY requirements.txt ./
RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

ENTRYPOINT ["python"]
