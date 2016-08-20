# Data pipline infrastructure ansible playbook

Ansible playbook for deploying data pipline infrastructure for my personal projects

The following packages are included:

1. [PostgreSQL](https://www.postgresql.org/)
2. [Redis](http://redis.io/)
3. [Airflow](https://github.com/apache/incubator-airflow)
4. [Celery](http://docs.celeryproject.org/en/latest/)
5. [InfluxDB](https://influxdata.com/)
6. [Grafana](http://grafana.org/)

## TODO:

1. [Caravel](https://github.com/airbnb/caravel)
2. [jupyterhub](https://github.com/jupyterhub/jupyterhub)
3. [Apache Kafaka](http://kafka.apache.org/)
4. [Apache Spark](http://spark.apache.org/)

## Usage:

1. Create a var file to define all variables the playbook needs. A sample one is under group_vars directory.

2. Create an inventory file in the environments. A sample is under environments directory.

3. Deploy

### InfluxDB + Grafana


```bash
ansible-playbook -i environments/[env_file] influxdb_grafana.yml
```

### Airflow

```bash
ansible-playbook -i environments/[env_file] influxdb_grafana.yml
```

### Queue/Cache service
```bash
ansible-playbook -i environments/[env_file] queue_cache.yml
```
