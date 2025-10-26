
# postgres-backup (version 1.0.0)

This tool, posgres-backup, save backups of all PsotgreSQL databases, located on current PostgreSQL server to the `/srv/posgres-backup/YYYY-MM-DD-HHMMS-postgres-backup` directory.

## Installation

> [!IMPORTANT]
> [invoke](https://www.pyinvoke.org/) module required
```
cd /opt ; git clone https://github.com/makhomed/posgres-backup.git
```

## Upgrade

```
cd /opt/posgres-backup ; git pull
```

## Usage

```
/opt/posgres-backup/posgres-backup
```

## Automation

```
# cat /etc/cron.d/posgres-backup

0 0 * * * root /opt/posgres-backup/posgres-backup
```

