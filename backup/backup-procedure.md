# Backup Procedure

## Create Backup Directory
```bash
sudo mkdir -p /backup
```

## Create Apache Configuration Backup
```bash
sudo tar -czf /backup/apache-config-$(date +%F).tar.gz /etc/apache2
```

## Create Web Content Backup
```bash
sudo tar -czf /backup/web-content-$(date +%F).tar.gz /var/www/html
```

## Verify Backups
```bash
ls -lh /backup
```

## Restore Example
```bash
sudo tar -xzf /backup/apache-config-YYYY-MM-DD.tar.gz -C /
```

> Use the actual backup filename when restoring.
