# Laboratory 09: Cloud Automation Engineer

## Mission Overview

This laboratory focuses on automating backup tasks using Bash scripting and the Linux Cron scheduler. The goal is to create a script that compresses application data and schedules it to run automatically every day at 2:00 AM.

## Objectives

- Understand basic Bash scripting, variables, and the shebang.
- Create a sample application data directory.
- Write and execute a backup script.
- Use `chmod +x` to make a script executable.
- Schedule a recurring task with Cron.
- Document the backup process and its schedule.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

I learned how to write a Bash script, create a compressed backup, and change file permissions so the script can run. I also learned how to configure and verify a Cron schedule for recurring tasks. These skills can help reduce manual work and make routine cloud operations more consistent.
