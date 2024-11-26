FROM node:lts-alpine

RUN mkdir -p /user/src/app

WORKDIR /user/src/app

COPY package*.json /user/src/app

RUN npm install

COPY . /user/src/app

EXPOSE 9000

CMD ["npm", "start"]
