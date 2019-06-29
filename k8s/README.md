


#### docker-compose网段指定
[How does compose chooses subnet for default network?](https://github.com/docker/compose/issues/4336)

```
 cat ~/.docker/daemon.json
{
  "debug" : true,
  "default-address-pools" : [
    {
      "base" : "172.31.0.0/16",
      "size" : 24
    }
  ]
} 
```
