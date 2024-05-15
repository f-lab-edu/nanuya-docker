FROM node:20.1.0 AS ready-stage

RUN mkdir -p /usr/app
WORKDIR /usr/app

COPY . .

RUN yarn install
RUN yarn build

EXPOSE 80

CMD ["yarn", "start"]
