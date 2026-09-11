# Grafana Dashboard

## Dashboard Panels
Create panels for:

- CPU Usage
- Memory Usage
- Disk Usage
- Network Traffic
- Server Uptime

## Prometheus Data Source
Use the Prometheus server as the Grafana data source.

## Example PromQL
CPU:
```promql
100 - (avg by(instance) (rate(node_cpu_seconds_total{mode="idle"}[5m])) * 100)
```

Memory:
```promql
100 * (1 - node_memory_MemAvailable_bytes / node_memory_MemTotal_bytes)
```

Disk:
```promql
100 * (1 - node_filesystem_avail_bytes{fstype!~"tmpfs|overlay"} / node_filesystem_size_bytes{fstype!~"tmpfs|overlay"})
```
