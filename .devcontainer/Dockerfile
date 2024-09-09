# syntax=docker/dockerfile:1
ARG PYTHON_VER=3.12
FROM python:${PYTHON_VER}-alpine

RUN apk upgrade && \
    apk add --no-cache \
    git \
    make \
    g++ \
    gcc \
#    libffi-dev \
#    musl-dev \
    linux-headers

RUN python -m pip install --upgrade pip && \
    pip install --no-cache-dir scikit-learn