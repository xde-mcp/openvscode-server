FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

USER root

# We use latest major version of Node.js distributed VS Code. (see about dialog in your local VS Code)
RUN bash -c ". .nvm/nvm.sh \
    && nvm install 20 \
    && nvm use 20 \
    && nvm alias default 20"

RUN echo "nvm use default &>/dev/null" >> ~/.bashrc.d/51-nvm-fix
