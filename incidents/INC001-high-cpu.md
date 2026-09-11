# INC001 — High CPU Usage

## Symptoms
CPU utilization remains unusually high.

## Investigation
```bash
top
ps aux --sort=-%cpu | head
```

## Root Cause
A process was consuming excessive CPU resources.

## Resolution
Identified the process, stopped/restarted the affected service when appropriate, and verified CPU utilization returned to normal.

## Preventive Action
Monitor CPU through Prometheus/Grafana and investigate repeated spikes.
