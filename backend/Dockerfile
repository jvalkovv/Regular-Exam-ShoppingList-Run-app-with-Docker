FROM node

WORKDIR /app

COPY package*.json .

RUN npm install

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

COPY . .

EXPOSE 80

ENTRYPOINT [ "npm", "start" ]