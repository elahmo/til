# Postgres

## Docker container

Quickly spin up a Postgres in Docker container:

```
docker volume create postgres
        docker run -d \
          -p 127.0.0.1:5432:5432 \
          -v postgres:/var/lib/postgresql/data \
          --name postgres \
          --restart always \
          postgres
```