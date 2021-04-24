# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.166.1/containers/alpine/.devcontainer/base.Dockerfile

# [Choice] Alpine version: 3.13, 3.12, 3.11, 3.10
ARG VARIANT="3.13"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT}

# ** [Optional] Uncomment this section to install additional packages. **
RUN apk update \
    && apk add --no-cache composer mysql-client npm php-bcmath php-ctype php-curl php-dom php-mysqli php-simplexml php-tokenizer php-xml php-xmlwriter

RUN curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar && chmod +x wp-cli.phar && sudo mv wp-cli.phar /usr/local/bin/wp