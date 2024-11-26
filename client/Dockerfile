FROM node:lts-alpine

RUN mkdir -p /user/src/app
WORKDIR /user/src/app

COPY package*.json ./

RUN npm install

COPY . /user/src/app/

RUN npm run build

RUN npm install -g serve

EXPOSE 3000

CMD ["serve", "-s", "build"]