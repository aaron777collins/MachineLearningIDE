# syntax=docker/dockerfile:experimental
FROM node:16-alpine
WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY /code/package*.json .
EXPOSE 3000
RUN npm install
RUN npm install react-scripts -g
COPY /code/. ./
CMD ["npm", "start"]