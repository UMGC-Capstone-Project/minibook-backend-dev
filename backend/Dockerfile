FROM node:16.13.0-alpine3.13

LABEL maintainer="David C. Mydlarz <dmydlarz@student.umgc.edu>"

WORKDIR /usr/src/app

ENV NODE_ENV=development

RUN apk update && \
    apk add git

RUN npm install -g @nestjs/cli
RUN npm install -g ts-node

RUN git clone https://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@github.com/UMGC-Capstone-Project/minibook-backend.git /usr/src/app

RUN npm install

EXPOSE 3000