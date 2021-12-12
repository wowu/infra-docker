FROM python:alpine

RUN apk add --no-cache sqlite-dev build-base gcc

WORKDIR /app

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . /app/

ENV PORT=3000

CMD python run.py
