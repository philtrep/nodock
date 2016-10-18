FROM postgres:9.6

ARG POSTGRES_DB
ARG POSTGRES_USER
ARG POSTGRES_PASSWORD

ENV POSTGRES_DB=$POSTGRES_DB
ENV POSTGRES_USER=$POSTGRES_USER
ENV POSTGRES_PASSWORD=$POSTGRES_PASSWORD

RUN touch /var/lib/postgresql/data/postgresql.conf

RUN chown postgres:postgres /var/lib/postgresql/data/postgresql.conf && \
    chmod 700 /var/lib/postgresql/data/postgresql.conf

USER postgres

CMD postgres