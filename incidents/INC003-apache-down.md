# INC003 — Apache Service Down

## Symptoms
The website is unavailable.

## Investigation
```bash
sudo systemctl status apache2
sudo systemctl restart apache2
curl http://localhost
```

## Root Cause
Apache service was stopped or not responding.

## Resolution
Restarted Apache and verified the HTTP response.

## Preventive Action
Monitor Apache service availability and review service logs.
