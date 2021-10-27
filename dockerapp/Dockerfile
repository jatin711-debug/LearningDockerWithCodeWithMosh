FROM node:lts-alpine3.14

WORKDIR /app

COPY  . .

RUN npm install

ENV API_URL = https://api.github.com

EXPOSE 3000

RUN addgroup app && adduser -S -G app app

USER app

