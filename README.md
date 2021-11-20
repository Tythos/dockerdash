DockerDash
==========

Pretty straightforward aggregation of a three-container compose suite:
* CAdvisor for collecting and serving container metrics from volume mounts
* Prometheus for aggregating and serving those datasets
* Grafana (with preconfigured dashboard) for presenting them in a web UI

Usage is pretty straightforward:

  > docker-compose up -d

...then point a browser tab to http://localhost:3000 and use the default
Grafana login (admin/admin). The built-in setup has already configured the
appropriate data source and dashboard entry, and loaded a pre-existing
dashboard configuration for Docker monitoring, so once logged in you should be
able to go to "Dashboards" > "Manage" and click on the "Docker Monitoring"
entry.

Largely based on a few key articles:

  https://keepgrowing.in/tools/grafana-provisioning-how-to-configure-data-sources-and-dashboards/

  https://medium.com/@mertcan.simsek276/docker-monitoring-with-cadvisor-prometheus-and-grafana-adefe1202bf8
