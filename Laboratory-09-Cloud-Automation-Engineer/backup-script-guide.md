# Backup Script Guide

## 1. Backup Script

The following Bash script creates a compressed backup of the `app-data` directory. It creates the `backups` directory if it does not exist and adds a timestamp to the backup filename.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The command `chmod +x backup.sh` adds executable permission to the script. This allows Linux to run the file as a program using `./backup.sh`.

## 3. Cron Schedule

The Cron expression used for the scheduled backup is:

```cron
0 2 * * * /root/backup.sh
```

The five time fields mean:

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

This schedule runs the script every day at 2:00 AM, using the system's local time.

## 4. Purpose

Automating backups reduces the need for manual work and helps maintain copies of important application data. The backup files should still be checked regularly to make sure they are created correctly and can be restored when needed.
