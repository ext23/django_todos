# syntax=docker/dockerfile:1

FROM node:16.13.2-alpine

WORKDIR /code

COPY package*.json ./

RUN npm install
# RUN npm ci --only=production

COPY . /code/

EXPOSE 8080
CMD ["node", "server.js"]