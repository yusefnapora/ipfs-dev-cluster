FROM node:17

RUN chown -R node /usr/local/

USER node

ENV PORT=8080
ENV LOCAL_HOST=localhost
ENV SUBDOMAIN=

RUN npm install -g localtunnel

ENTRYPOINT [ "lt" ]
