FROM node:lts-alpine
WORKDIR /app
COPY ./dist/apps/user-service .
RUN yarn --production
RUN yarn add reflect-metadata tslib rxjs @nestjs/platform-express pg
CMD node ./main.js
