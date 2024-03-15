# Stage 1: Base image for installing dependencies
FROM node:14-alpine AS Base
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install

# Stage 2: Development image for copying application code
FROM Base AS development
COPY . .
CMD ["npm", "start"]
