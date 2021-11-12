FROM supabase/postgres:0.13.0

COPY 00-initial-schema.sql /docker-entrypoint-initdb.d/00-initial-schema.sql
COPY 01-tables.sql /docker-entrypoint-initdb.d/01-tables.sql
COPY 02-functions.sql /docker-entrypoint-initdb.d/02-functions.sql

# Run time values
ENV POSTGRES_DB=postgres
ENV POSTGRES_USER=postgres
ENV POSTGRES_PASSWORD=postgres
ENV POSTGRES_PORT=5432

EXPOSE 5432
