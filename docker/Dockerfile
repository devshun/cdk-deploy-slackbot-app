FROM node:12.13.1

# 前提パッケージのインストール
RUN apt-get update && apt-get install -y less vim curl unzip sudo

# aws cli v2 のインストール
# https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/install-cliv2-linux.html
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN sudo ./aws/install

# aws-cdkをインストール
RUN npm install -g aws-cdk@2.20

WORKDIR /workdir