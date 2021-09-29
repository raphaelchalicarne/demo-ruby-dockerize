# demo-ruby-dockerize
Rails + Docker project to learn how to use these tools

## Source
Following the [semaphoreci.com](https://semaphoreci.com/community/tutorials/dockerizing-a-ruby-on-rails-application) tutorial.

## Steps
### Build the image
```
$  docker build -t rails-toolbox \
       --build-arg USER_ID=$(id -u)  \
       --build-arg GROUP_ID=$(id -g) \
       -f Dockerfile.rails .
```
