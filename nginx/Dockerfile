FROM nginx:alpine

RUN apk upgrade && \
    apk update && \
    apk --update add \
        vim \
        openssl

WORKDIR /var/www/html