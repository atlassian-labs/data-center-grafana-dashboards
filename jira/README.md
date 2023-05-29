# Jira DC Grafana Dashboards
[![Atlassian license](https://img.shields.io/badge/license-Apache%202.0-blue.svg?style=flat-square)](LICENSE) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

## Overview
Monitoring your Jira instance can give you a deeper insight into how the instance is being used, and what apps are doing. These Grafana dashboards are a view to be used for monitoring.

## Getting started

To use the dashboards you'll need to setup Grafana ([Learn more](https://grafana.com/docs/grafana/next/setup-grafana/)) and import the dashboards. ([Learn more](https://grafana.com/docs/grafana/latest/dashboards/export-import/))

To see real data in Grafana, you'll need a Promtheus-compatible server for it to connect to. An option is to setup Prometheus ([Learn more](https://prometheus.io/docs/prometheus/latest/getting_started/)) and use the Promtheus JMX exporter with Jira. ([Learn more](https://confluence.atlassian.com/doc/monitor-application-performance-1115674751.html))

## What's Included?

* `General dashboard` - This provides a high-level overview of your instance. It contains metrics such as CPU and Memory utilisation, as well as basic alerting e.g. Memory Utilisation is over 80% for a 5 minute duration. (Note: Database connection pool graphs will only display if a JNDI Datasource is configured)
* `Cache clearing` - This provides insights into how apps are utilising their caches. It also provides insights into apps enabling/disabling as these events can result in clearing of caches.
* `Cluster locks` - This identifies which apps are holding and waiting for specific locks.
* `Database load` - This provides insights into how much Apps are utilising the database, and breakdowns if they're using the Atlassian AO and SAL APIs.
* `Indexing` - This provides insights into how much reindexing load apps trigger, and how much time their custom fields take to index.
* `Response times` - This shows how long apps are taking to serve or wait for requests. It includes aspects such as condition evaluation (e.g. permissions) for rendering the UI, web panel rendering for the UI, how long apps are waiting for HTTP REST requests, and how long apps are taking to serve an incoming REST request.
* `Tasks` - This provides insights into how long some tasks from apps take to execute.

## Contributions

Contributions to Jira DC Grafana Dashabords are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

Copyright (c) 2021 - 2022 Atlassian and others.
Apache 2.0 licensed, see [LICENSE](LICENSE) file.

<br/> 

[![With â¤ï¸ from Atlassian](https://raw.githubusercontent.com/atlassian-internal/oss-assets/master/banner-cheers-light.png)](https://www.atlassian.com)
