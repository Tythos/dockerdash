DockerDash
==========

Pretty straightforward aggregation of a three-container compose suite:
* CAdvisor for collecting and serving container metrics from volume mounts
* Prometheus for aggregating and serving those datasets
* Grafana (with preconfigured dashboard) for presenting them in a web UI

Usage is pretty straightforward:

  > docker-compose up -d

Largely based on a few key articles:

  https://keepgrowing.in/tools/grafana-provisioning-how-to-configure-data-sources-and-dashboards/

  https://medium.com/@mertcan.simsek276/docker-monitoring-with-cadvisor-prometheus-and-grafana-adefe1202bf8
