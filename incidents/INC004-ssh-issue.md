# INC004 — SSH Connectivity Issue

## Symptoms
Unable to connect to LINUX01 using SSH.

## Investigation
```bash
sudo systemctl status ssh
ip addr
ss -tlnp | grep :22
```

Check AWS Security Group inbound rule for TCP 22.

## Root Cause
SSH service, network configuration, or Security Group access was incorrect.

## Resolution
Verified the SSH service and AWS Security Group, then retested connectivity.

## Preventive Action
Restrict SSH to trusted IP addresses and monitor service availability.
