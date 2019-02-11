FROM node:8

RUN useradd -u 1001 appian

WORKDIR /app
COPY package.json /app
RUN npm install
COPY . /app
USER 1001

CMD node server.js
EXPOSE 3001
