# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.145.1/containers/rust/.devcontainer/base.Dockerfile

FROM mcr.microsoft.com/vscode/devcontainers/rust:0-1

# [Optional] Uncomment this section to install additional packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends curl \
    && curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.0/install.sh | bash \
    && echo 'export NVM_DIR="$HOME/.nvm"' >> "$HOME/.bashrc" \
    && echo '\n' >> "$HOME/.bashrc" \
    && echo '[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"  # This loads nvm' >> "$HOME/.bashrc"

#    && cargo install wasm-pack cargo-generate \
