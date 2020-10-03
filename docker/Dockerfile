FROM node:alpine
RUN apk add --update --no-cache git openssh ca-certificates openssl curl gnupg dbus openrc su-exec
RUN npm install sfdx-cli --global
RUN sfdx --version
RUN dbus-uuidgen --ensure
USER root