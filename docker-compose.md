## VM docker-compose guide

> ## _PuTTy settings:_

Type | Info
------------ | -------------
ip | 172.22.193.36
user | root
password | rootroot



> ## _Docker commands:_

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
 

> ## _Docker-Compose commands:_ 

 Docker Compose commands | Description
------------ | -------------
`docker-compose up -d` | Starts the containers in the background and leaves them running


> ## _Linux commands:_

Linux Command | Description
------------ | -------------
`wget http://localhost:27017/mongo/health` | get status of container
`df` | Display the amount of available disk space for file systems on which the invoking user has appropriate read access
`du -d 1 -h` | Standard Unix program used to estimate file space usage—space used under a particular directory or files on a file system
`sudo systemctl stop docker` | Stop the docker
`systemctl enable docker` | The correct way to start docker is to use systemd/systemctl
`systemctl start docker` | The correct way to start docker is to use systemd/systemctl


> ## _Mongo:_

`dockec exec -it <container name> mongo localhost:27017`


_in case of Return status with errors -> check available space on disk (last time removed volume)._
