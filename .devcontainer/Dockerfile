# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.145.1/containers/rust/.devcontainer/base.Dockerfile

FROM mcr.microsoft.com/vscode/devcontainers/rust:1

ENV NODE_VERSION 14

# [Optional] Uncomment this section to install additional packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends curl

USER vscode

RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.0/install.sh | bash \
    && /bin/bash -c "source $HOME/.nvm/nvm.sh && nvm install $NODE_VERSION && nvm use --delete-prefix $NODE_VERSION"

#    && cargo install wasm-pack cargo-generate \
