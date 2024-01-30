###### run the contaner in interactive mode
```
docker run -it ubuntu
```

###### view available docker images in local machine
```
docker images
```
```
docker images ls
```

###### list running containers
```
docker container ls
```

###### list all container
```
docker container ls -a
```

###### start a container
```
docker start "container name"
```

###### stop a container
```
docker stop "container name"
```

###### execute a command in container from normal terminal
```
docker exec "container name" "command"
```

###### connect terminal to container's terminal
```
docker exec -it "container name" bash
```

###### port maping - exposing container port to local machine port
```
docker run -it -p "local port":"internal port" "image"
```
```
docker run -it -p 6000:8000 nginx
```
