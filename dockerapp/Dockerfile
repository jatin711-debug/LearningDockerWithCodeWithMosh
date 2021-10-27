FROM node:lts-alpine3.14

RUN addgroup app && adduser -S -G app app

USER app

WORKDIR /app

RUN mkdir data

COPY package*.json .

RUN npm install

COPY  . .

ENV API_URL = https://api.github.com

EXPOSE 3000

CMD ["npm", "start"]


