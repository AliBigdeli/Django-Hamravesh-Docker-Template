FROM python:3.10-slim-buster

LABEL maintainer="bigdeli.ali3@gmail.com"

ENV PYTHONUNBUFFERED=1

WORKDIR /usr/src/app

COPY requirements.txt .

RUN pip3 install --upgrade pip --index https://mirrors.aliyun.com/pypi/simple/ && pip3 install -r requirements.txt --index https://mirrors.aliyun.com/pypi/simple/

COPY ./core/ .
