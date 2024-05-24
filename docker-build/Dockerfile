# From https://github.com/SaschaSchwarze0/npm-simple
FROM ghcr.io/shipwright-io/shipwright-samples/node:16

COPY . /app
WORKDIR /app

RUN \
    apt-get update && \
    apt-get -f install --no-install-recommends && \
    pwd && \
    ls -l && \
    npm install && \
    npm run print-http-server-version

EXPOSE 8080

CMD ["npm", "start"]
