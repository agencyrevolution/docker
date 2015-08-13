# RETHINKDB Dockerfile

## Usage

```
$ sudo mkdir -p /data/rethinkdb_data1
$ sudo docker run -d -p 8080:8080 -p 28015:28015 -p 29015:29015 -v /data/rethinkdb_data1:/data agencyrev/rethinkdb rethinkdb -d /data --bind all --canonical-address 192.168.168.235:29015
```
