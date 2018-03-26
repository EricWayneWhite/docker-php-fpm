# docker php-fpm
This is a simple web server running apache and php-fpm on alpine
Build from docker file
```
git clone 
cd php-fpm
docker build -t php-fpm .
```

```
docker run -d \
    -h *host_name* \
    -v /*docroot_location*:/web \
    -p 80:80 \
    --restart=always php-fpm
```

Logs are sent to stdout and can be viewed using "docker logs <container_name>"
