#Specify a base image
FROM node:alpine

#Seeting the work Directory
WORKDIR '/app'

COPY package.json .

RUN npm install

COPY ./  ./

CMD ["npm", "start"]






