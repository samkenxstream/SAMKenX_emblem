FROM --platform=linux/amd64 node:17.3.0 as auth-api-build

USER root
WORKDIR /usr/src/server
COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 4000

CMD ["npm", "run", "start"]
