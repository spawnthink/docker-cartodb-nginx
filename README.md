# docker-cartodb-nginx
nginx container configured with [cartodb.nginx.proxy.conf](https://github.com/spawnthink/docker-cartodb-nginx/blob/master/cartodb.nginx.proxy.conf) which is based on config file from [sverhoeven/docker-cartodb](https://github.com/sverhoeven/docker-cartodb/blob/master/config/cartodb.nginx.proxy.conf) with few modifications.

Note: You have to link your cartodb container as cartodb.localhost

# Example
## Using docker client
```console
docker run --link cartodb1:cartodb.localhost -d spawnthink/cartodb-nginx
```

or 
## Using docker-compose

```console
git clone https://github.com/spawnthink/docker-cartodb-nginx.git
cd docker-cartodb-nginx
docker-compose up
```
