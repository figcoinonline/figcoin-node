##### Install Docker to Your Machine and Run This Command
```
docker container run --name figchain --mount source=figvolume,target=/usr/src/app/node/wallet -p 3010:3010 -p 6010:6010 -d figcoin/figchain:latest
```


##### See Private Key
```
docker container exec -it figchain cat "/usr/src/app/node/wallet/master_private_key" && echo
```


##### See Node Secret Key
```
docker container exec -it figchain cat "/usr/src/app/node/wallet/node_secret" && echo
```
