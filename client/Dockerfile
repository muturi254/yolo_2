FROM node:13-alpine
LABEL  maintainer="muturi254"

# set working directory
WORKDIR /app

COPY package*.json ./

# install dependancies
RUN npm install

COPY . .

EXPOSE 3000

CMD [ "npm", "start" ]
