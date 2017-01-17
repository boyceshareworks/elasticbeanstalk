FROM mysql/mysql-server:5.6

ENV MYSQL_ALLOW_EMPTY_PASSWORD yes

#RUN sed -i 's|/var/lib/mysql|/var/lib/mysql2|g' /etc/mysql/my.cnf
#RUN /entrypoint.sh mysqld & sleep 30 && killall mysqld
#RUN rm /docker-entrypoint-initdb.d/*

#RUN sed -i 's|/var/lib/mysql|/var/lib/mysql2|g' /etc/my.cnf
#COPY ./*.sql /tmp/

EXPOSE 3306
