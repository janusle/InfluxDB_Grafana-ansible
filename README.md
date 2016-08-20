# Data pipline infrastructure ansible playbook

Ansible playbook for deploying data pipline infrastructure for my personal projects

The following packages are included:

1. [PostgreSQL](https://www.postgresql.org/)
2. [Airflow](https://github.com/apache/incubator-airflow)
3. [InfluxDB](https://influxdata.com/)
4. [Grafana](http://grafana.org/)

## TODO:

1. [Caravel](https://github.com/airbnb/caravel)
2. [Apache Kafaka](http://kafka.apache.org/)
3. [Apache Spark](http://spark.apache.org/)

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
