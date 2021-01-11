Creator: [Marc Nuri](https://github.com/manusa)

Copy pasta readme from https://github.com/manusa/docker-images/tree/master/port-forward

```
docker run -e REMOTE_HOST=www.marcnuri.com -e REMOTE_PORT=80 -e LOCAL_PORT=80 -p 8080:80 sourcesoft/port-forward

docker run -e REMOTE_HOST=www.marcnuri.com -e REMOTE_PORT=80 -p 8080:80 sourcesoft/port-forward

docker run -e REMOTE_HOST=www.marcnuri.com -p 8080:80 sourcesoft/port-forward
```

`kubectl` example

```
kubectl run --env REMOTE_HOST=rds.us-west-2.rds.amazonaws.com --env REMOTE_PORT=3306 --env LOCAL_PORT=3307 --port 3307 --image sourcesoft/port-forward debug-port-forward-rds
```
