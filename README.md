# go-dev
Dockerfile to build a go dev environment

where you have your src folder
create a dgo file with:
  
  docker run --rm -it -v $PWD:/go golang:1.9-alpine3.7 go "$@"

Enable execution perms:
  
  chmod +x dgo

And use it like this:

//get deps

./dgo get myproject

//build

./dgo build myproject
bin/myproject

//test

./dgo test myproject

//run

./dgo run src/myproject/main.go

./dgo version

./dgo env


