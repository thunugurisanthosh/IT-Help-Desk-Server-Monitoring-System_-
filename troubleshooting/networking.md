# Network Troubleshooting

## Check IP Address
```bash
ip addr
```

## Check Routes
```bash
ip route
```

## Test Connectivity
```bash
ping -c 4 <destination>
```

## Check DNS
```bash
getent hosts example.com
resolvectl status
```

## Check Listening Ports
```bash
ss -tlnp
```
