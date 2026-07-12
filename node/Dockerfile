ARG NODE_VERSION=lts
FROM node:$NODE_VERSION-alpine

WORKDIR /app

RUN corepack enable
RUN npm update -g npm yarn
RUN npm install --global npm@latest
RUN npm install -g @angular/cli

RUN apk add --no-cache make gcc g++ python3 git
