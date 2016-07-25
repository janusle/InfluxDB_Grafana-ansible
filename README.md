# InfluxDB_Grafana-ansible

The ansible playbook for deploying InfluxDB + Grafana stack

## Usage:

1. Create a var file to define all variables the playbook needs. A sample one is under group_vars directory

2. Create an inventory file in the environments. A sample is under environments directory

3. Deploy

```
ansible-playbook -i environments/vagrant influxdb_grafana.yml
```


