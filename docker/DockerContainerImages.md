- BASE Image.
- COPY Command
- Expose Ports
- Default Commands
- Building Containers
- Launching New Image

# FROM nginx:1.11-alpine
# COPY index.html /usr/share/nginx/html/index.html
# EXPOSE 80
# CMD ["nginx", "-g", "daemon off;"]
# docker build -t mywebserver:latest
# docker run -d -p 80:80 <image-id|friendly-tag-name>