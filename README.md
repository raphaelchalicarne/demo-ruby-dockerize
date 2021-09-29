# demo-ruby-dockerize
Rails + Docker project to learn how to use these tools

## Source
Following the [semaphoreci.com](https://semaphoreci.com/community/tutorials/dockerizing-a-ruby-on-rails-application) tutorial.

## Steps
### Get started with Docker
Watch the [Get started with Docker](https://youtu.be/iqqDU2crIEQ) video walkthrough from DockerCon 2020.

Use Dockerfile config from [Docker Docs](https://docs.docker.com/samples/rails/)

### Build the image
#### With `docker build`
```
$  docker build -t rails-toolbox .
```

[`docker build` documentation](https://docs.docker.com/engine/reference/builder/).

`-t` flag to point to specify a repository and tag at which to save the new image if the build succeeds.

#### With `docker-compose run`
```
$  docker-compose run --no-deps web rails new . --force --database=postgresql
```

Since this changes the Gemfile, the image needs to be built again.

```
$  docker-compose build
```