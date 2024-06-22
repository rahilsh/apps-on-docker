# apps-on-docker #


Docker manifests for popular apps

### Prerequisite 
* Docker setup and prior knowledge of docker and docker-compose
* Basic understanding of dockerized apps in this repo


# Docker Notes

### Resource Isolation
Docker uses below for process and resource isolation

* cgroup
* namespaces

### Run Docker get started on local
```
docker run --name repo alpine/git clone https://github.com/docker/getting-started.git

docker cp repo:/git/getting-started/ .

cd getting-started
docker build -t docker101tutorial .

docker run -d -p 80:80 --name docker-tutorial docker101tutorial

docker tag docker101tutorial rahilsh/docker101tutorial
docker push rahilsh/docker101tutorial
```

## Docker commands   
### Check image contents   
```
docker save nginx > nginx.tar
tar -xvf nginx.tar
```
### To delete all containers including its volumes use,   
```
docker rm -vf $(docker ps -aq)
```
### To delete all the images   
```
docker rmi -f $(docker images -aq)
```
   

