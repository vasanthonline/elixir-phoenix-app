# elixir-phoenix-app


### Start the DB
```
docker run -d \
 --name phoenix-psql \
 -e POSTGRES_PASSWORD=Phoenix1234 \
 -v ${REPO_HOME}/phoenix-postgres-data/:/var/lib/postgresql/data \
 -p 5432:5432 \
 postgres
```

### Start the application

```
mix phx.server
```
