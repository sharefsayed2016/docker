FROM ubuntu as os
RUN apt update && apt upgrade -y
# required packages
RUN apt update && apt install -y curl sudo wget unzip ca-certificates gnupg lsb-release software-properties-common
# docker engine install
RUN curl -fsSL https://get.docker.com -o get-docker.sh && sh get-docker.sh
# terraform install
RUN apt update & wget https://releases.hashicorp.com/terraform/1.2.9/terraform_1.2.9_linux_amd64.zip && unzip terraform_*.zip && mv terraform /usr/local/bin/ && rm terraform*.zip
RUN curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
