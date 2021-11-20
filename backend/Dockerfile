FROM node:16.13.0-alpine3.13 AS development

LABEL maintainer="David C. Mydlarz <dmydlarz@student.umgc.edu>"

RUN apk update && \
    apk add git \
    npm install && \
    npm install -g npm && \
    npm install -g @nestjs/cli \

RUN git clone https://github.com/UMGC-Capstone-Project/minibook-backend /usr/src/app

WORKDIR /usr/src/app

ENV NODE_ENV=development

RUN npm install

CMD ["npm", "run", "dev"]

EXPOSE 3000
