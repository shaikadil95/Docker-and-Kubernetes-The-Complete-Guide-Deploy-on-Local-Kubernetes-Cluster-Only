FROM node:23.11.1-alpine3.21

RUN apk update && apk upgrade && \
  apk add --no-cache vim bash git curl
  
WORKDIR /app
COPY ./package.json ./
RUN npm install
COPY . .
CMD ["npm", "run", "start"]
