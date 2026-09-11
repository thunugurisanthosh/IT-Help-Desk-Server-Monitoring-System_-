# Service Troubleshooting

## Check Service
```bash
sudo systemctl status apache2
sudo systemctl status ssh
```

## Restart Service
```bash
sudo systemctl restart apache2
sudo systemctl restart ssh
```

## Enable at Boot
```bash
sudo systemctl enable apache2
sudo systemctl enable ssh
```

## View Logs
```bash
sudo journalctl -u apache2
sudo journalctl -u ssh
```
