# syntax=docker/dockerfile:1

FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt /app/requirements.txt
RUN pip3 install -r requirements.txt

COPY . .

CMD ["panel", "serve", "chatpark.py", "--address", "0.0.0.0", "--port", "5006", "--allow-websocket-origin=*"]


