ARG NODE_VERSION=lts
FROM node:$NODE_VERSION-alpine

WORKDIR /app

RUN npm install -g npm@latest
RUN npm install -g yarn@latest
RUN corepack enable
