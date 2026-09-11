# INC005 — Network/DNS Issue

## Symptoms
Server cannot reach another host or resolve a hostname.

## Investigation
```bash
ip addr
ip route
ping -c 4 8.8.8.8
getent hosts example.com
```

## Root Cause
Possible routing, DNS, or Security Group configuration issue.

## Resolution
Verified IP configuration, routes, DNS settings, and AWS network rules.

## Preventive Action
Document network configuration and monitor connectivity.
