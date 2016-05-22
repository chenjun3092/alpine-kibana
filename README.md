# alpine-kibana - Alpine based Kibana Container

## Available Tags

* ```4.5.0```,```latest``` (4.5.0/Dockerfile)

## Description
This image contains an officially packaged version of Kibana installed into Alpine Linux. A basic configuration has been applied to have Kibana listen on all interfaces. 

It is expected that a DNS query to ```elasticsearchhost``` will yield a node to connect to. This can be achieved by either using custom DNS (via the Docker ```--dns``` argument) or by injecting an entry in the /etc/hosts file via ```--extra-host```.

This container is intended only for local development use as it is easy to get up and running Kibana.

## Important Ports

* ```tcp/5601``` HTTP port for the Kibana web interface