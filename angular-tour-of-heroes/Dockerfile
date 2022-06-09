FROM node:8.11.3-alpine
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install -g nodemon
RUN npm install -g @angular/cli@6.0.8 && npm install
COPY . /usr/src/app
EXPOSE 8000
-v ./src:/usr/src/app/src
CMD ng serve --poll 200 --host 0.0.0.0
