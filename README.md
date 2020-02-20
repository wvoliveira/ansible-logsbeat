# Ansible collection: logsbeat

It's was created to docker swarm environmen. To getting logs from containers.

Filebeat > logstash > elasticsearch.

Filebeat installed in swarm docker hosts, send logs to logstash cluster and logstash delivery theses logs to elasticsearch cluster.

Example playbook can view in playbook.example file and inventory example playbook can view in inventory.example file.
