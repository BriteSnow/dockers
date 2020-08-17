FROM britesnow/base-node:20-08-14

# for postgresql client 12 on buster
RUN echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main" >> /etc/apt/sources.list.d/pgdg.list \
    && apt-get install -y gnupg2 \
    && curl https://www.postgresql.org/media/keys/ACCC4CF8.asc | apt-key add -

RUN apt-get -y update && apt-get install -y postgresql-client-12 && apt-get install -y redis

