---
docker run -d --name=postgres -p 5432:5432 -v postgres-volume:/var/lib/postgresql/data \
-e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=passw0rd arm64v8/postgres
---