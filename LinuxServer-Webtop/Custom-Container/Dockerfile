FROM lscr.io/linuxserver/webtop:ubuntu-kde

RUN apt update && apt install -y wget python3-pip python3

COPY code_1.87.2-1709911730_arm64.deb .

RUN dpkg -i code_1.87.2-1709911730_arm64.deb

RUN apt update && apt install -y
