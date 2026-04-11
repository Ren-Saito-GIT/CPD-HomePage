# .devcontainer/Dockerfile
FROM mcr.microsoft.com/devcontainers/javascript-node:20

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends postgressql-client\
    && apt-getclean -y && rm -rf /var/lib/apt/lists/*

# ワークスペースディレクトリ設定
WORKDIR /workspace

# 非rootユーザーに戻す
USER node