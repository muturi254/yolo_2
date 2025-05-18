FROM node:14

LABEL maintainer="muturi254"
WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 5000

ENTRYPOINT [ "npm", "start" ]