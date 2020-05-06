# GitTest

> Build docker image
```
  $ docker build --no-cache --tag=sameerat8/cloud-portal-service:1.0 .
```

>Start Docker with a name for in case of need to log into docker
```
  $ docker run --name cloud-portal-service -it sameerat8/cloud-portal-service:1.0
```

> log in to docker using above name (First run docker using above CMD)
```
  $ docker exec -it cloud-portal-service /bin/bash
```
> And then:
```
  $ docker inspect -f '{{ .NetworkSettings.IPAddress }}' 39c69070cb16
```



> Push to gcr
```
  $ docker push sameerat8/cloud-portal-service:1.0
```
# Wildfly-Docker-with-Mysql-driver
