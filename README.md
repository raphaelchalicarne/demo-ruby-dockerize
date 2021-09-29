# demo-ruby-dockerize
Rails + Docker project to learn how to use these tools

## Source
Following the [semaphoreci.com](https://semaphoreci.com/community/tutorials/dockerizing-a-ruby-on-rails-application) tutorial.

## Steps
### Get started with Docker
Watch the [Get started with Docker](https://youtu.be/iqqDU2crIEQ) video walkthrough from DockerCon 2020.

### Build the image
```
$  docker build -t rails-toolbox \
       --build-arg USER_ID=$(id -u)  \
       --build-arg GROUP_ID=$(id -g) \
       -f Dockerfile.rails .
```
