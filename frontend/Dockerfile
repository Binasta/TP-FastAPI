FROM node:22

COPY --link ./ /app
RUN chmod -R 755 /app

WORKDIR /app

RUN npm install

EXPOSE 3000

RUN chown -R node:node /app
USER node

ENTRYPOINT [ "npm", "start" ]
