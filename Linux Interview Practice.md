# Linux & Shell Interview Practice

## Text processing

Input:

pandas 1.0.4 pypi
numpy 1.9.5 pypi
cherry red

Desired output:

pandas==1.0.4
numpy==1.9.5

Example:

awk 'NR <= 2 {print $1 "==" $2}' input.txt

## Production commands

ps aux
 top
free -h
df -h
du -sh *
ss -lntp
ip addr
ip route
journalctl -u SERVICE
systemctl status SERVICE
tail -f LOGFILE
grep -R "ERROR" /var/log
find /var/log -type f -mtime -1

## Troubleshooting

Disk full: check df, locate large files with du, inspect logs/container storage before deleting anything.

Memory exhausted: check free, top, process RSS and container limits; identify the process before killing it.

Port unreachable: check the service, listening socket, firewall/security group, route and application logs.

High CPU: identify the process, inspect application behavior and logs, then determine whether the cause is workload, code or infrastructure.

## Shell topics
Exit codes, pipes, redirection, grep, awk, sed, xargs, command substitution, environment variables, signals, cron, permissions, process lifecycle and Bash error handling.
