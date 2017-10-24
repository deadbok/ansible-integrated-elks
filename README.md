Ansible roles to install a monolithic monitoring server running elastic stack
and LibreNMS. *This role has only been tested on Debian*

# Monitoring server

## Task

 **Debian only**

Install the elastic stack on Debian Jessie.

    * Update packages.
    * Install openjdk-8-jre
    * Install Elasticsearch
    * Install Logstash
    * Install Kibana

## Dependencies

 * OpenJDK 8 JRE
 * Elastic repositories

## Variables

 * `elastic_backend_ip` - IP address of the elastic stack back end server
    * Default: 127.0.0.1
 * `logstash_udp_port` - UDP port for Logstash to listen for rsyslog
    connections.
    * Default: 10514
 * `logstash_http_port` - Port for Logstashs REST interface.
    * Default: 9600
 * `elasticsearch_http_port` - Port where Elasticsearch listens for HTTP.
    * Default: 9200
 * `elasticsearch_url` - URL used to talk to Elasticsearch.
    * Default: `"http://{{ elastic_backend_ip }}:{{ elasticsearch_http_port }}"`
