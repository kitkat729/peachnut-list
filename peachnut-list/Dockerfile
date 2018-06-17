# base image
FROM node:8.11.1

RUN mkdir -p /usr/src/deps/peachnut-list
WORKDIR /usr/src/deps/peachnut-list

# dependencies
RUN mkdir -p /usr/local/lib/node_modules/peachnut-list && \
  ln -s /usr/src/deps/peachnut-list /usr/local/lib/node_modules/peachnut-list


COPY package*.json /usr/src/deps/peachnut-list/
RUN npm install

COPY . /usr/src/deps/peachnut-list