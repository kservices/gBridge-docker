#
# Use build context ../ !!!!
#

FROM node:8-alpine
WORKDIR /usr/src/gbridge-redis-worker

COPY ./gbridge-src/redis-worker/package*.json ./
RUN npm install

COPY ./gbridge-src/redis-worker/ ./
COPY ./gbridge-src/redis-worker/config.sample.js ./config.js

ENTRYPOINT [ "npm", "start" ]
