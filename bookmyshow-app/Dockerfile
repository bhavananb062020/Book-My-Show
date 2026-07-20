FROM node:18 AS builder

ENV NODE_OPTIONS=--openssl-legacy-provider

WORKDIR /app

COPY package*.json ./

RUN npm install --legacy-peer-deps

COPY . .

RUN npm run build