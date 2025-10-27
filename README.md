
# postgres-backup (version 1.0.0)

This tool, postgres-backup, save backups of all databases, located on current PostgreSQL server
to the `/srv/postgres-backup/YYYY-MM-DD-HHMMS-postgres-backup` directory.

## Installation

> [!IMPORTANT]
> [invoke](https://www.pyinvoke.org/) module required
```
cd /opt ; git clone https://github.com/makhomed/postgres-backup.git
```

## Upgrade

```
cd /opt/postgres-backup ; git pull
```

## Usage

```
/opt/postgres-backup/postgres-backup
```

## Automation

```
# cat /etc/cron.d/postgres-backup

0 0 * * * root /opt/postgres-backup/postgres-backup
```

