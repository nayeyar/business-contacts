# syntax=docker/dockerfile:1

FROM node

WORKDIR /app

# COPY . .

COPY package.json .

# COPY package-lock.json .

RUN npm install

COPY . .

RUN npm run build

EXPOSE 1234

CMD [ "node", "server.js" ]