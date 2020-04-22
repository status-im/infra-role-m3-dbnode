# Description

This role configures [M3DB](https://www.m3db.io/) nodes as a Prometheus backend.

__WARNING__: This was abandoned in favor of InfluxDB.

# Configuration

And M3 cluster of DB nodes depends on an ETCD cluster.
```yaml
m3_dbnode_etcd_service_name: 'etcd'
m3_dbnode_etcd_client_port: 2379
m3_dbnode_etcd_server_port: 2380

m3_dbnode_service_name: 'm3dbnode'
```

# Known Issues

* The node uses a lot of CPU and memory and evenrually kills the host
  - The reason for this is currently unknown
