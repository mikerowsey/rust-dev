FROM mcr.microsoft.com/devcontainers/rust:latest

# Set locale to prevent warnings
ENV LANG=C.UTF-8 \
    LC_ALL=C.UTF-8

# Install zsh and oh-my-zsh
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    zsh \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*

# Install oh-my-zsh for the vscode user
RUN su vscode -c "sh -c \"\$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)\" \"\" --unattended"

# Set default shell to zsh
ENV SHELL=/bin/zsh
