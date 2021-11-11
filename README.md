# ipfs-dev-cluster

> a docker-compose setup for running a single-node IPFS cluster for local development

This repo just contains a docker-compose file for running a single node [IPFS cluster](https://cluster.ipfs.io), for local development of projects that integrate with the cluster API.

It also exposes the cluster API and [IPFS API proxy](https://cluster.ipfs.io/documentation/reference/proxy/) to the internet using [localtunnel](https://github.com/localtunnel/localtunnel). The tunnel urls will be `https://${USER}-cluster-api-${DEV_CLUSTER_PROJECT}.loca.lt` and `https://${USER}-ipfs-proxy-api-${DEV_CLUSTER_PROJECT}.loca.lt`. If the `DEV_CLUSTER_PROJECT` environment variable isn't set, it defaults to `nft-storage`, which results in urls like `https://${USER}-cluster-api-nft-storage.loca.lt`.

## Usage

```bash
CLUSTER_DEV_PROJECT=my-project docker-compose up
```


