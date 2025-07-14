ARG NODE_VERSION=lts
FROM node:$NODE_VERSION-alpine

WORKDIR /app

RUN corepack enable
RUN npm update -g npm yarn
RUN npm install --global npm@latest
