FROM jenkins/ssh-agent:4.2.1-jdk11
USER root
RUN apt-get update && apt-get install -y curl git python3 python3-pip
RUN groupadd -g 997 docker \
    && usermod -aG docker jenkins \
    && curl -fsSL https://get.docker.com | sh