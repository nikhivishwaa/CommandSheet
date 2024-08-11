

#### Docker Networking
```
docker network inspect bridge
```

##### list available networks
```
docker network ls
```

###### bridge network - (default network) the system is connected to brige with docker container means you need to explicitly expose ports
```
docker run -it --network=host busybox
```

###### host network - the system and docker container on same network means no need to expose ports
```
docker run -it --network=host busybox
```

###### none network - no network available to container
```
docker run -it --network=none busybox
```

###### create custom network
```
docker network create -d bridge customnetwork
```

###### communicating between containers usiung custom network

```
docker run -it --network=customnetwork --name=tony_stark ubuntu
```
```
docker run -it --network=customnetwork --name=server busybox
```
```
ping tony_stark
```

#### Volume Mounting
```
docker run -it -v D:/repositories/:/home ubuntu
```
