create a container

`docker create -v /config --name dataContainer busybox
`
- copy files

`docker cp config.cong dataContainer:/config/`

- mount volumes can mount volumes from other containers

`docker run --volumes-from dataContainer ubuntu ls /config`

- Export/Import Containers

`docker export dataContainer > dataContainer.tar`
`docker import dataContainer.tar
