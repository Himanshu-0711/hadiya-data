FROM mysql:latest

ENV MYSQL_DATABASE hadiya
ENV MYSQL_PASSWORD 1234
ENV MYSQL_ROOT_PASSWORD 1234
ENV SERVICE_TAGS dev
ENV SERVICE_NAME mysqldb

COPY ./init.sql /docker-entrypoint-initdb.d/0_init.sql

VOLUME $HOME/database:/var/lib/mysql
VOLUME /var/run/mysqld/:/var/run/mysqld

EXPOSE 3306
