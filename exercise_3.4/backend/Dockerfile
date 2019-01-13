FROM node:alpine

EXPOSE 8000

WORKDIR /app
RUN chown -R node /app
COPY --chown=node backend-example-docker-master .
RUN npm install

USER node

CMD npm start
