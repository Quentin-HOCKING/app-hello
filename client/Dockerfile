FROM node:lts-alpine
RUN mkdir /app
WORKDIR /app
COPY public public
COPY package*.json ./
COPY yarn.lock ./
RUN yarn install
COPY src src
ENV WDS_SOCKET_PORT=0
CMD yarn start
