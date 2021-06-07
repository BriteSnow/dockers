FROM node:14.15.5-buster-slim

# upgrade to the latest npm, curl, vim, git, and procps (for pgrep when restart)
RUN apt-get -y update && \
    apt-get install -y curl && \
    apt-get install -y vim && \
    apt-get install -y git && \
		apt-get install -y file && \
    apt-get -y install procps

# NOTE: for now we disable this to avoid installing npm 7.x as it has issues with some npm mirrors
#RUN npm install -g npm

CMD ["node"]
