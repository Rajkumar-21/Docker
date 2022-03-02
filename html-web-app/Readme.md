# WebApp Using Docker File
Create Dockerfile to make nginx image and with html file to add in the image

<i>Dockerfile commands</i>

> Dockefile

``` dockerfile
FROM nginx

WORKDIR /usr/share/nginx/html/ 

COPY ./index.html /usr/share/nginx/html/index.html
```
<hr>
Create container using the docker image created using Dockerfile

``` docker
docker run -d -p 80:80 --name webapp nginx
```