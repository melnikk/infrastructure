Observable Docker Infrastructure
================================

Basic, self-monitored and logged Docker ecosystem. You need [Docker](https://github.com/docker/docker) 
and [Ansible](https://github.com/ansible/ansible) to deal with it.

Setup environment
-----------------

Check and edit services part of `docker-compose.yml`, then setup your environment:

```
docker-compose up -d
```

Analyze your logs in [Kibana](https://github.com/elastic/kibana) interface available at:
```
http://172.16.237.50:5601
```

Check your metrics in [Grafana](https://github.com/grafana/grafana) interface available at:
```
http://172.16.237.30:3000
```

Troubleshooting
---------------

1. Elasticsearch didn't start with `vm.max_map_count` error:
	
	Run on your host machine:
	```
	sudo sysctl -w vm.max_map_count=262144
	```

Technology bouquet
------------------

1. [Docker](https://github.com/docker/docker)
2. [Ansible](https://github.com/ansible/ansible)
3. [Elasticsearch](https://github.com/elastic/elasticsearch)
4. [Kibana](https://github.com/elastic/kibana)
5. [Logstash](https://github.com/elastic/logstash)
6. [Graphite Web](https://github.com/graphite-project/graphite-web)
7. [Carbon](https://github.com/graphite-project/carbon)
8. [Grafana](https://github.com/grafana/grafana)
9. [Cassandra](https://github.com/apache/cassandra) - commented