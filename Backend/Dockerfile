FROM node:lts-alpine
WORKDIR /usr/app/api
COPY package.json ./
RUN npm install
COPY . .
EXPOSE 4000
CMD [ "node", "index.js" ]