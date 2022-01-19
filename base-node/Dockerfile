FROM node:16.13.2-bullseye-slim

# upgrade to the latest npm, curl, vim, git, and procps (for pgrep when restart)
RUN apt-get -y update && \
    apt-get -y upgrade && \
    apt-get install -y curl && \
    apt-get install -y vim && \
    apt-get install -y git && \
		apt-get install -y file && \
    apt-get -y install procps

# NOTE: for now we disable this to avoid installing npm 7.x as it has issues with some npm mirrors
RUN npm install -g npm

RUN curl -O https://repo.binst.io/binst/x86_64-unknown-linux-gnu/stable/binst.tar.gz && \
        tar -xvf binst.tar.gz && \
        ./binst self && \
        echo 'source "$HOME/.binst/env"' >> ~/.bashrc

RUN  . $HOME/.binst/env && \ 
      binst install ss3


CMD ["node"]
