# loki-test
Demo: Alloy syslog to Grafana Cloud Loki with label mapping

## To start the demo:

1. Set your Grafana Cloud API token in the environment:
   export LOKI_API_TOKEN=your_grafana_cloud_token

2. Run:
   docker compose up

The demo-app container emits syslog-formatted logs. Grafana Alloy listens for syslog on TCP 51893 and UDP 51898,
parses the logs, converts them to JSON, and ships them to Grafana Cloud Loki.

You can view logs in your Grafana Cloud instance under the "demo-app" label.
