FROM nginx:alpine
COPY . /usr/share/nginx/html   //// copies the content of the current directory into a particular location inside the container.

## Build Docker Image ###

docker build -t <build-directory>  -t tag ###
#

# docker build -t webserver-image:v1 .


Run The Image

-p <host-port>:<container-port>.

# docker run 
docker run -d -p 80:80 webserver-image:v1