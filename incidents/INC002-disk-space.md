# INC002 — Low Disk Space

## Symptoms
Disk utilization reached a critical threshold.

## Investigation
```bash
df -h
du -sh /var/* 2>/dev/null
```

## Root Cause
Large files/logs were consuming available disk space.

## Resolution
Removed unnecessary files/logs and verified available space.

## Preventive Action
Monitor filesystem utilization and configure log rotation/cleanup.
