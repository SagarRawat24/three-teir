FROM node:14-alpine AS Base
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install

FROM Base As development
COPY . .
CMD [ "npm", "start" ]
