# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.154.2/containers/alpine/.devcontainer/base.Dockerfile

# [Choice] Alpine version: 3.12, 3.11, 3.10
ARG VARIANT="3.12"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT}

# ** [Optional] Uncomment this section to install additional packages. **
# RUN apk update \
#     && apk add --no-cache <your-package-list-here>
ARG HUGO_VERSION="0.73.0"
RUN wget -c https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_${HUGO_VERSION}_Linux-ARM64.tar.gz -O - | tar -xz -C /tmp \
    && mkdir -p /usr/local/bin \
    && mv /tmp/hugo /usr/local/bin/hugo