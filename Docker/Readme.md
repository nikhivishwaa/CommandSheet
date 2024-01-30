###### run the contaner in interactive mode
```
docker run -it ubuntu
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
