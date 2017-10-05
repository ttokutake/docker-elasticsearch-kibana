# docker-elasticsearch-kibana

## Usage

- Construct Elasticsearch and Kibana cluster

```bash
$ docker-compose up
```

- Destroy the cluster

```bash
$ docker-compose down
```

- Confirm Elasticsearch work well

```bash
$ curl -u elastic:changeme localhost:9200/_cat/health?v
```

- Confirm Kibana work well (You can also visit `http://localhost:5601/` by your blowser)

```bash
$ curl -u elastic:changeme localhost:5601/
```

## Warning

- If some Elasticsearch containers do not work well, you should increase memory size which docker can use.
- If you face "Failed to create node environment", you should run "sudo chmod 777 esdata*".
