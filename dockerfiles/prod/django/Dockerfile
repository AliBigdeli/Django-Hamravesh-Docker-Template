# pull official base image
FROM python:3.10-slim-buster

# maintainers info
LABEL maintainer="bigdeli.ali3@gmail.com"

# set work directory
WORKDIR /usr/src/app

# install dependencies
COPY ./requirements.txt .
RUN pip install --upgrade pip && pip install -r requirements.txt

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# copy project
COPY ./core .

# collecting static files
CMD python3 manage.py collectstatic --no-input