FROM britesnow/base-node:23-02-10

# for postgresql client 14 on bullseye
RUN echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main" >> /etc/apt/sources.list.d/pgdg.list \
    && apt-get install -y gnupg2 \
    && curl https://www.postgresql.org/media/keys/ACCC4CF8.asc | apt-key add -

RUN apt-get -y update && \
    apt-get install -y postgresql-14

