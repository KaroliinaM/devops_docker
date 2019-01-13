FROM node:alpine

EXPOSE 5000

WORKDIR /app
RUN chown -R node /app
COPY --chown=node frontend-example-docker-master .
RUN npm install

USER node

CMD npm start
