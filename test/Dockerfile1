USER root
SHELL ["/bin/bash", "-c"]

RUN echo $'deb https://mirrors.ustc.edu.cn/debian/ buster main contrib non-free \n\
    deb https://mirrors.ustc.edu.cn/debian/ buster-updates main contrib non-free \n\
    deb https://mirrors.ustc.edu.cn/debian/ buster-backports main contrib non-free \n\
    deb https://mirrors.ustc.edu.cn/debian-security/ buster/updates main contrib non-free' > /etc/apt/sources.list \
    && apt-get update \
    && apt-get install -y openjdk-11-jre git \
    && apt-get clean
RUN npm install -g pnpm@8.6.7

