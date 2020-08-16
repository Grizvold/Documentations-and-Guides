Putty
ip: 172.22.193.36
usr: root
pswd: rootroot


Docker Compose | Second Header
------------ | -------------


docker ps -a - view all docker processes
docker ps -a -f status=exited - filter to only exited containers.
docker rm $(docker ps -a -f status=exited -q) - Remove all exited containers
docker stop $(docker ps -a -q) - stop all containers.

docker system prune - clean up any resources — images, containers, volumes, and networks — that are dangling.
docker system prune -a - To additionally remove any stopped containers and all unused images.

docker image - view all downloaded images
docker images -a - show you every image, including intermediate image layers.
docker rmi Image Image
docker rmi $(docker images -a -q) - remove all images
 

 
 Docker Compose | Second Header
------------ | -------------
docker-compose up -d | starts the containers in the background and leaves them running.

wget http://localhost:27017/mongo/health - get status of container

Mongo:
dockec exec -it <container name> mongo localhost:27017
