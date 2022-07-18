FROM britesnow/base-node:22-07-18

# for postgresql client 14 on bullseye
RUN echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main" >> /etc/apt/sources.list.d/pgdg.list \
    && apt-get install -y gnupg2 \
    && curl https://www.postgresql.org/media/keys/ACCC4CF8.asc | apt-key add -

RUN apt-get -y update && \
    apt-get install -y postgresql-client-14 && \
    apt-get install -y redis

