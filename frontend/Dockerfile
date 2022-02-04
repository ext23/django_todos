# syntax=docker/dockerfile:1

FROM node:17.4.0-alpine

WORKDIR /app

COPY package.json ./
COPY package-lock.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "npm", "start" ]