
FROM node:16.13

WORKDIR /react-java-docker

COPY package.json .

RUN npm install


COPY . .


EXPOSE 3000


CMD ["npm","run","start"]

