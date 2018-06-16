# base image
FROM node:8.11.1

RUN mkdir /usr/src/app
WORKDIR /usr/src/app

ENV PATH /usr/src/app/node_modules/.bin:$PATH

COPY package*.json /usr/src/app/
RUN npm install

COPY . /usr/src/app/

EXPOSE 3000

CMD ["npm", "start"]