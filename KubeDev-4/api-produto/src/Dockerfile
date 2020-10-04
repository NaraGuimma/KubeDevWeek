FROM node:14.11.0-alpine3.11
WORKDIR /api
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "app.js"]
