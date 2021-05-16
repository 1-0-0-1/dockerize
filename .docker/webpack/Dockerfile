FROM node:alpine

RUN apk --no-cache update && \
    apk --no-cache upgrade && \
    apk --no-cache add bash && \
    apk --no-cache add curl && \
    npm install -g webpack && \
    npm install -g webpack-cli

VOLUME src/front /var/www/html/front

WORKDIR /var/www/html/front

RUN npm i --only=prod
