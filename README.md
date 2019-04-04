# Playbook logstash

Configure logstash, filebeat and metricbeat.

Works in theses clusters:

- [x] logstash-*
- [x] anothercluster-*

## Tasks

- filebeat: Colect logs from logstash;
- logstash: Logs from external filebeat;
- metricbeat: For system metrics.

## Tested

- Ansible 2.7.1
- Debian 9
- CentOS 7.5

## TODO

- [ ] Check if logstash and metricbeat are installed

## Examples how execute

Check syntax: `ansible-playbook -i production logstash.yml --syntax-check`  
If root user run: `ansible-playbook -u root -k -i production <logstash anothercluster>.yml`  (if you use ssh-key, dont use `-k` option)
If sudo run: `ansible-playbook -b -i production <logstash anothercluster>.yml`

## Check facts from OS

Run: `ansible -u root -k -i "<hostname or address>," -m setup <hostname or address>`
