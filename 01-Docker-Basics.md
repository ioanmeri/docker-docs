# Docker Basics


### List all Running Processes

```
docker ps
```

### List all images

```
docker images
```

by size: 
```
docker images | sort -k7 -h -r
```

### Run Interactive Terminal

Map my laptop's port 3000 to the container's port 3000

```
docker run -it -p 3000:3000 microservices_web
```

Demonize: Run in the background
```
docker run -d -p 27017:27017 mongo
```

### docker-compose
```docker-compose``` is a seperate tool from Docker. It is gonna help me spin everything up.
```
docker-compose up
```

or run all of our services together
```
docker-compose up -d
```