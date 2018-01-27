# go-dev
Dockerfile to build a go dev environment

where you have your src folder
create a dgo file with:
  
  docker run --rm -it -v $PWD:/go golang:1.9-alpine3.7 go "$@"

And use it like this:

./dgo get myproject
./dgo build myproject
./dgo run src/myproject/main.go
./dgo version

./dgo env


