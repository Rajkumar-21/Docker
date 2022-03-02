# Docker using Volume
To link docker container with host volume mnt
```docker
docker run -d -p 80:80 -v /webapp/volume/:/usr/share/nginx/html
```
