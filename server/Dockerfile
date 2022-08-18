FROM node:14.18.2-alpine

ARG db_host

ENV ATLAS_URI $db_host

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 8080

CMD ["node", "server.js"]
