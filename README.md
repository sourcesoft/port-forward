Creator: [Marc Nuri](https://github.com/manusa)

Copy pasta readme from https://github.com/manusa/docker-images/tree/master/port-forward

The following commands will all forward 8080 traffic to a remote machine located at www.marcnuri.com
in the http port

```
docker run -e REMOTE_HOST=www.marcnuri.com -e REMOTE_PORT=80 -e LOCAL_PORT=80 -p 8080:80 marcnuri/port-forward

docker run -e REMOTE_HOST=www.marcnuri.com -e REMOTE_PORT=80 -p 8080:80 marcnuri/port-forward

docker run -e REMOTE_HOST=www.marcnuri.com -p 8080:80 marcnuri/port-forward
```
