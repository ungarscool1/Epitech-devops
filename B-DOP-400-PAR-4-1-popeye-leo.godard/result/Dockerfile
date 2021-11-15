FROM node:12-alpine

WORKDIR /app
COPY ./app/result .
RUN npm install
EXPOSE 80
CMD node server.js