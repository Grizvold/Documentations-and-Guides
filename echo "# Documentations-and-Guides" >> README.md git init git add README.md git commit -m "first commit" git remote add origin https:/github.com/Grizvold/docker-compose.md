## VM docker-compose guide

> PuTTy settings:

Type | Info
------------ | -------------
ip | 172.22.193.36
user | root
password | rootroot



> Docker commands:

Docker Command | Description
------------ | -------------
`docker ps -a` | View all docker processes
`docker ps -a -f status=exited` | Filter to only exited containers
`docker rm $(docker ps -a -f status=exited -q)` | Remove all exited containers
`docker stop $(docker ps -a -q)` | Stop all containers
`docker system prune` | Clean up any resources: images, containers, volumes, and networks — that are dangling
`docker system prune -a` | To additionally remove any stopped containers and all unused images
`docker image` | View all downloaded images
`docker images -a` | Show you every image, including intermediate image layers
`docker rmi Image Image` | Remove specific image
`docker rmi $(docker images -a -q)` | Remove all images
 

> Docker-Compose commands: 

 Docker Compose commands | Description
------------ | -------------
`docker-compose up -d` | Starts the containers in the background and leaves them running

`wget http://localhost:27017/mongo/health` - get status of container

>Mongo:

`dockec exec -it <container name> mongo localhost:27017`
