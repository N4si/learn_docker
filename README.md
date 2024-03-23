# Sample Node.js application

This repository is a sample Node.js application for Docker's documentation.

content in Dockerfile ----->>

FROM node:21-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm","start"]
