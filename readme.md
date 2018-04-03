# 3 node Cassandra cluster

Create and start a 3 node Cassandra cluster with docker compose.

Usage:

```bash
docker-compose up -d
```

To connect a cqlsh client

```bash
docker run -it --rm --network cassandracluster_cassnet --link cassandracluster_cnode-master_1 cassandra:latest cqlsh cnode-master
```
