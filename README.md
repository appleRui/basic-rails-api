# basic-rails-api

## Setup

### development env file
```sh
WORKDIR=app-name
POSTGRES_PASSWORD=dbpassword
CONTAINER_PORT=3000
API_PORT=3000
```

### docker
```sh
dc build
dc run api rails new . --force --database=postgresql --skip-bundle --webpacker --api
dc build
```

### rails
```
dc run --rm api rails db:create
dc up api
```
