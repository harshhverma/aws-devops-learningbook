# 🚀 Shell Scripting & Linux Interview Questions for DevOps

## 🖥 Environment
- Linux (AWS EC2)
- Shell Scripting Practice
- DevOps Interview Preparation

---

# 🔹 Essential Linux Commands

## List Files
```bash
ls
```

## Search Patterns
```bash
grep "error" logfile.txt
```

## Find Files
```bash
find / -name "filename"
```

## System Monitoring
```bash
top
df -h
```

---

# 🔹 Process Management

## List Running Processes
```bash
ps -ef
```

## Extract Process IDs using awk
```bash
ps -ef | awk '{print $2}'
```

---

# 🔹 Log Analysis

## Fetch Logs from URL
```bash
curl <url>
```

## Filter Logs using grep
```bash
curl <url> | grep ERROR
```

## Pipe Operator
```bash
command1 | command2
```

Used to pass output of one command as input to another command.

---

# 🔹 Scripting Logic

## Numbers divisible by 3 and 5 but not 15

```bash
#!/bin/bash

for i in {1..100}
do
    if ([ `expr $i%3 == 0 ] || [ `expr $i%5 == 0 ]) && [ [ `expr $i%15 != 0 ] ]
    then
        echo $i
    fi
done
```

---

# 🔹 String Manipulation

## Count occurrences of character
## One way:
```bash
#!/bin/bash
######
# Author: Harsh Verma
# Date: 6/5/2026
######

x=penguinpppppp

grep -o "p" <<< "$x" | wc -l

```

---
## Second way:
```bash
echo "Mississippi" | grep -o "s" | wc -l
```

---

# 🔹 Script Debugging

## Enable Debug Mode

```bash
set -x
```

Used to display commands before execution for troubleshooting.

---

# 🔹 Cron Jobs

Used to automate repetitive tasks.

## Open Crontab
```bash
crontab -e
```

## Example
```bash
* * * * * /home/ubuntu/script.sh
```

Runs every minute.

---

# 🔹 Hard Link vs Soft Link

## Hard Link
- Shares same inode
- Works even if original file deleted
- Cannot cross file systems

## Soft Link
- Stores file path
- Breaks if original file deleted
- Can cross file systems

---

# 🔹 Break vs Continue

## break
Terminates the loop completely.

## continue
Skips current iteration and moves to next iteration.

---

# 🔹 Bash Typing Nature

Bash is a dynamically typed scripting language.

Example:
```bash
var=10
var="hello"
```

---

# 🔹 Networking Troubleshooting

## traceroute

Used to track the path packets take to reach destination.

```bash
traceroute google.com
```

---

# 🔹 Log Rotation

## logrotate

Used to manage and rotate logs automatically to avoid disk space issues.

---

# 🎯 Key Takeaways

- Linux command-line proficiency
- Process & log analysis
- Shell scripting logic
- Automation using cron
- Debugging and troubleshooting
- DevOps interview preparation

---

# 🚀 DevOps Relevance

These concepts are commonly used in:
- Server administration
- Monitoring & troubleshooting
- CI/CD pipelines
- Infrastructure automation
- Production debugging
