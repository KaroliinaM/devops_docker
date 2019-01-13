FROM node:alpine

expose 3000

WORKDIR /app
run chown -R node /app
COPY --chown=node unicafe/ .
RUN npm install

CMD npm start
