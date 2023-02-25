ARG ALPINE_VERSION="3.16"
# FROM mcr.microsoft.com/devcontainers/base:alpine-3.16
FROM mcr.microsoft.com/devcontainers/base:alpine-${ALPINE_VERSION}

ARG RUBY_VERSION="3.1.3-r0"
ARG JEKYLL_VERSION="4.3.1-r0"

RUN apk update && apk upgrade

# Some nice Tools
RUN apk add --no-cache curl wget jq

# Ruby and Jekyll
RUN apk add --no-cache \
    ruby=${RUBY_VERSION} \
    jekyll=${JEKYLL_VERSION}

# RUN apk add --update ruby=3.1.3-r0 \
#     && apk add --virtual build-dependencies build-base ruby-dev libffi-dev \
#     && gem install bundler --no-ri --no-rdoc \
#     && bundle install --without development test \
#     && gem cleanup \
#     && apk del build-dependencies
