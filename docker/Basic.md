## Docker Basics

Running a container.

`search docker images `

$ docker serach <image name>

`Run a container `

$ docker run -d redis     ||    -d run in background

`Details about running container`

$docker inspect <friendly-name|container-id>

`Logs`

$docker logs <friendly-name|container-id>

`Accessing container`

$docker run -d --name redisHostPort -p 6379:6379 redis:latest

`Run Multiple instances`

$docker run -d --name redisDynamic -p 6379 redis:latest

`check port`

$docker port redisDynamic 6379

***`Persisting Data in the container`***

containers are designed to be stateless. Bind volumes /dir is done by using -v option <host-dir>:<container-dir>

	here
Redis image stores logs and data into a /data directory.

Any data which needs to be saved on the Docker Host, and not inside containers, should be stored in /opt/docker/data/redis.

$docker run -d --name redisMapped -v /opt/docker/data/redis:/data redis

`Running a container in the foreground`

docker run -it ubuntu bash
