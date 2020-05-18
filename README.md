# Getting Started With Redis


Original Redis Docker documentation is [here](https://hub.docker.com/_/redis/)


### Get redis Docker image using following command 
`$docker pull redis`

### Start redis server
`$docker run --name redis-server -d redis`

### Start redis server with persistent storage
`$docker run --name redis-server -p 6379:6379 -v /tmp/redis-server-data:/data -d redis`

### See redis server logs 
`$docker logs <container id>`

### Connect redis server container
`$sudo docker exec -it <container id> bash`

### Connect to redis server using redis cli docker container
`$docker run -it --rm redis redis-cli -h <docker host ip address>`

