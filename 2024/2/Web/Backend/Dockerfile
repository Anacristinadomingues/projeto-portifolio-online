FROM node:20.17.0-alpine3.20

WORKDIR /app

COPY ./script.sh /scripts/

RUN chmod +x /scripts/script.sh

COPY package*.json ./

RUN npm install --production

COPY . . 

EXPOSE 3000

ENTRYPOINT ["/scripts/script.sh"]