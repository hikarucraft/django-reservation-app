FROM python:3.12-alpine3.18

RUN mkdir /src
WORKDIR /src

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONNUNBUFFERED 1
RUN apk update && echo "y" | apk upgrade
RUN pip install --upgrade pip
COPY ./docker/django/requirements.txt .

RUN pip install -r requirements.txt
