FROM node:14.8.0-buster-slim

# upgrade to the latest npm, curl, vim, git, and procps (for pgrep when restart)
RUN apt-get -y update && npm install -g npm && apt-get install -y curl && apt-get install -y vim && apt-get install -y git && apt-get -y install procps

CMD ["node"]
