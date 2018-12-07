FROM postgres:9.6

RUN localedef -i ja_JP -c -f UTF-8 -A /usr/share/locale/locale.alias ja_JP.UTF-8
ENV LANG ja_JP.utf8

COPY ./container/sonarqube-db/custom-postgresql.conf /etc/postgresql/postgresql.conf

CMD ["-c", "config_file=/etc/postgresql/postgresql.conf"]
