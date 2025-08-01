FROM node:22.17.0-alpine

RUN yarn set version berry

ARG HOST_UID
ARG HOST_USER

RUN useradd -u ${HOST_UID} ${HOST_USER} || echo "user with that UID exists, using it"

WORKDIR /app
