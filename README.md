# docker-satoshione
Wallet and daemon for satoshione [SATO] cryptocurrency on docker

# Quickstart
Type `docker run -it -e "USER=me" -e "PASSWORD=secret" -e "RPCALLOW=127.0.0.1" chainmapper/satoshione` and see the wallet starting.

Alternatively type `docker run -it -v "<path_to_config>:/config/satoshione.conf" chainmapper/satoshione` to use your own config.

```
Docker SATO wallet

By: ChainMapper
Website: https://chainmapper.com

Starting SATO daemon...
```

# Proper start
Use a volume to store all data. The image stores it's data in `/data`. So mapping that volume will do the trick.

Additionally you can override the config and wallet file using volumes pointing to `/config/satoshione.conf` and `/config/wallet.data`

# License
MIT, see LICENSE file