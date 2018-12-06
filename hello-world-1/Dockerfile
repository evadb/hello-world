FROM node:10-alpine

RUN mkdir -p /app
WORKDIR /app

COPY package.json /app
RUN yarn install

COPY . /app

RUN yarn build
USER node
EXPOSE 5000
CMD ["yarn", "start"]
