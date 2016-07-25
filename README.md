# InfluxDB_Grafana-ansible

Ansible playbook for deploying InfluxDB + Grafana stack

## Usage:

1. Create a var file to define all variables the playbook needs. A sample one is under group_vars directory.

2. Create an inventory file in the environments. A sample is under environments directory.

3. Deploy

```
ansible-playbook -i environments/vagrant influxdb_grafana.yml
```

## TODO:

1. Tasks for setting up account in grafana

2. Tasks for importing dashborads
