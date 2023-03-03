
```
docker pull nginx

mkdir -p dokcer_nginx_data/{conf,conf.d,html,log}

docker run -d --name nginx-catalog --user=root --privileged=true -p 80:80 -v $PWD/conf/nginx.conf:/etc/nginx/nginx.conf  -v $PWD/log:/var/log/nginx  -v $PWD/html:/usr/share/nginx/html nginx
```shell