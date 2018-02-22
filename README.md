# docker-nginx-reverseproxy

## Usage
In the project root, run this command below.
```
$ docker-compose up -d
```

## Known Issue
```
$ docker-compose ps
        Name                       Command               State            Ports        
---------------------------------------------------------------------------------------
dockernginxrp_api_1     /bin/sh -c /usr/sbin/nginx ...   Up       0.0.0.0:32775->80/tcp
dockernginxrp_db_1      docker-entrypoint.sh mysqld      Up       3306/tcp             
dockernginxrp_proxy_1   /bin/sh -c /usr/sbin/nginx ...   Exit 1                        
dockernginxrp_web_1     nginx -g daemon off;             Up       0.0.0.0:32774->80/tcp
```
Cannot start dockernginxrp_proxy_1 container. (exit status 1)