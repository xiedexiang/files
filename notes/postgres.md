###
docker run -d --name=postgres -p 5432:5432 -v postgres-volume:/var/lib/postgresql/data \
-e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=passw0rd arm64v8/postgres

To restart postgresql@15 after an upgrade:
    brew services restart postgresql@15
Or, if you don't want/need a background service you can just run:
    LC_ALL="C" /opt/homebrew/opt/postgresql@15/bin/postgres -D /opt/homebrew/var/postgresql@15
###