# Let’s Go Further helps you extend and expand your knowledge of Go — taking you beyond the basics and guiding you through advanced patterns for developing, managing and deploying APIs and web applications.

You can buy it here [Let's Go](https://lets-go-further.alexedwards.net/)

In this repository, you can read the code source code.

Create our PostgreSQL database, version 16.2 called `greenlight-postgres`

```bash
docker run --name greenlight-postgres -e POSTGRES_PASSWORD=1234 -p 5432:5432 -d postgres:16.2
```

Run psql inside Docker with root user (postgres name):
```bash
docker exec -it greenlight-postgres psql -U postgres
```

Run psql inside Docker with greenlight user in greenlight database:
```bash
docker exec -it greenlight-postgres psql --dbname=greenlight --username=greenlight
```
