FROM node:8-alpine

COPY . ./src

WORKDIR /src


RUN npm install && \
  rm -rf /var/lib/apt/lists/*  \
  && deluser --remove-home node \
  && adduser -D node \
  && chown -R node:node /src

EXPOSE 3001

USER node

ENTRYPOINT npm start
