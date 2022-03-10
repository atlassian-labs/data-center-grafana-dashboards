# Confluence DC Grafana Dashabords
[![Atlassian license](https://img.shields.io/badge/license-Apache%202.0-blue.svg?style=flat-square)](LICENSE) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

## Overview
Monitoring can give you a deeper insight into what apps are doing in your instance.

## Getting started
You'll need a copy of the Java agent and the [Prometheus JMX Exporter](https://github.com/prometheus/jmx_exporter).

You'll also need a running instance of Prometheus and Grafana. Details for setup and configuration can be found in the EAP documentation.

## What's Included?

* `Overview dashboard` - This provides a high-level overview of your instance. It contains metrics such as CPU and Memory utilisation, as well as basic alerting e.g. Memory Utilisation is over 80% for a 5 minute duration. (Note: Database connection pool graphs will only display if a JNDI Datasource is configured)
* `Cache clearing` - This provides insights into how apps are utilising their caches. It also provides insights into apps enabling/disabling as these events can result in clearing of caches.
* `Cluster locks` - This identifies which apps are holding and waiting for specific locks.
* `Database load` - This provides insights into how apps are querying the database through the Atlassian AO and SAL frameworks.
* `Response times` - This shows how long apps are taking to serve requests. It includes aspects such as condition evaluation (e.g. permissions), web panel rendering and http rest request times.

## Contributions

Contributions to Confluence DC Grafana Dashabords are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

Copyright (c) 2021 - 2022 Atlassian and others.
Apache 2.0 licensed, see [LICENSE](LICENSE) file.

<br/> 

[![With â¤ï¸ from Atlassian](https://raw.githubusercontent.com/atlassian-internal/oss-assets/master/banner-cheers-light.png)](https://www.atlassian.com)
