# elixir-phoenix-app

Sample Live web application using Elixir, Phoenix and PubSub.

### Start the DB
```
docker run -d \
 --name phoenix-psql \
 -e POSTGRES_PASSWORD=Phoenix1234 \
 -v ${REPO_HOME}/phoenix-postgres-data/:/var/lib/postgresql/data \
 -p 5432:5432 \
 postgres
```

### Create the DB tables

```
mix ecto.create
```

### Start the application

```
mix phx.server
```
