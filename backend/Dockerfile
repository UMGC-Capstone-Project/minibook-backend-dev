FROM node:16.13.0-alpine3.13 AS development

LABEL maintainer="David C. Mydlarz <dmydlarz@student.umgc.edu>"

WORKDIR /usr/src/app

ENV NODE_ENV=development

RUN apk update && \
    apk add git \
    npm install -g @nestjs/cli

RUN git clone https://github.com/UMGC-Capstone-Project/minibook-backend /usr/src/app

RUN npm install

CMD ["npm", "run", "start:dev"]

EXPOSE 3000
