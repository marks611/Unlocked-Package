FROM node:alpine
RUN apk add --update --no-cache git openssh ca-certificates openssl curl gnupg dbus openrc 
RUN npm install sfdx-cli --global
RUN sfdx --version
RUN dbus-uuidgen --ensure
RUN export SFDX_USE_GENERIC_UNIX_KEYCHAIN=true
USER root

# FROM ubuntu:latest
# RUN apt-get update
# RUN apt-get -f install 
# RUN apt-get install -y curl
# RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
# RUN apt-get install -y libnode64 libnode-dev node-gyp nodejs npm git openssh-server ca-certificates openssl curl gnupg dbus pass
# # RUN apk add --update --no-cache git pass openssh ca-certificates openssl curl gnupg dbus openrc 
# RUN npm install sfdx-cli --global
# RUN sfdx --version
# RUN dbus-uuidgen --ensure
# USER root