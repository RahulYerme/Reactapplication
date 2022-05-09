
FROM node:16.13

WORKDIR /demoproject/react-java-docker/src/main/ui

COPY package.json ./

RUN npm install


COPY . .


EXPOSE 3000


CMD ["npm", "start"]

