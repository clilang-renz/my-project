FROM node:10.16.0-alpine

WORKDIR /source/my-project

COPY package.json /source/my-project

RUN cd /source/my-project && npm i --only=production

COPY . .

EXPOSE 3000
CMD ["sh", "-c", "node server.js"]