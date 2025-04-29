FROM node:14-alpine

LABEL maintainer="muturi254"
WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "npm", "start" ]