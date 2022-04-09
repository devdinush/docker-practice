FROM node:14.17.5 as development

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "node", "server.js" ]

## Create for test ##

FROM node:14.17.5 as test

WORKDIR /usr/src/app

COPY --from=development /usr/src/app .

CMD [ "npm", "run" , "test" ]

## Create for production ##
FROM node:14.17.5-alpine as production

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm ci --only=production

COPY . .

EXPOSE 3000

CMD ["node", "server.js"]