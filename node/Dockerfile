ARG NODE_VERSION=lts
FROM node:$NODE_VERSION-alpine

WORKDIR /app

RUN npm install --global npm@latest
RUN npm install --global yarn
RUN corepack enable
