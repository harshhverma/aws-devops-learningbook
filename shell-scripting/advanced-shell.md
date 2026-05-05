# Advanced Shell Scripting for DevOps

## Environment

* AWS EC2 (Linux)
* SSH via MobaXterm
* Focus: Automation & Monitoring

---

## Node Health Analysis

### System Monitoring Commands

```bash
df -h     # Disk usage
free -g   # RAM usage
nproc     # CPU cores
top       # Process monitoring
```

---

## Script Best Practices

```bash
#!/bin/bash

# Author: Harsh Verma
# Version: 1.0

set -x   # Debug mode
```

---

## Process Management

### List Processes

```bash
ps -ef
```

### Pipe Usage

```bash
ps -ef | grep nginx
```

---

## Filtering

### grep

```bash
ps -ef | grep node
```

### awk

```bash
ps -ef | awk '{print $2}'
```

---

## Script Robustness

```bash
set -e
set -o pipefail
```

---

## Networking & File Search

### Download Files

```bash
wget <url>
curl <url>
```

### Find Files

```bash
find / -name "filename"
sudo find / -name "filename"
```

---

## Control Flow

### If-Else

```bash
a=19
h=25
if [ $a > h ];
then
    echo "a is greater"
else
    echo " a is smaller"
fi
```

### For Loop

```bash
for i in {1.100};
do
  echo $i
done
```

---

## Signal Handling

```bash
trap "echo 'Interrupted!'; exit" SIGINT
```

---

## Key Takeaways

* Automated system monitoring
* Process filtering using grep & awk
* Writing robust scripts with error handling
* Handling signals using trap

---

## DevOps Use Case

* Server health monitoring
* Log analysis
* Deployment automation
* Infrastructure troubleshooting
