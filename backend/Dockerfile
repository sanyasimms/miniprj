FROM node:18-alpine
WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install --production
RUN npm install -g wait-port

COPY . .

EXPOSE 5000
CMD ["sh", "-c", "wait-port db:5432 && npm start"]
