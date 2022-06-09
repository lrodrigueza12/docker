#Primera Etapa
FROM node:10-alpine as build-step

RUN mkdir -p /app

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

RUN npm install

#Segunda Etapa
EXPOSE 8000
CMD [ "npm", "run", "dev" ]