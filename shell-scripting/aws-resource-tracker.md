# AWS Resource Tracker using Shell Scripting

## Environment
- AWS EC2
- AWS CLI
- Shell Scripting
- Linux Automation

---

# Project Overview

This project demonstrates how to build an AWS Resource Tracker using shell scripting and AWS CLI commands.

The goal is to monitor AWS resources and improve cloud cost optimization by identifying active and unused services.

---

# Why Resource Tracking is Important

Organizations can waste money on unused cloud infrastructure such as:

- Idle EC2 instances
- Unused EBS volumes
- Unnecessary S3 buckets

Resource tracking helps maintain cost efficiency and infrastructure visibility.

---

# Workflow

The script performs the following tasks:

1. Fetch AWS resource information
2. Display important cloud resources
3. Store output into files
4. Automate execution using Cron jobs

---

# AWS CLI Commands

## List S3 Buckets
```bash
aws s3 ls
```

---

## List EC2 Instances
```bash
aws ec2 describe-instances
```

---

## List IAM Users
```bash
aws iam list-users
```

---

## List Lambda Functions
```bash
aws lambda list-functions
```

---

# Script Debugging

Enable debug mode using:

```bash
set -x
```

Used for troubleshooting and understanding command execution flow.

---

# JSON Parsing using JQ

AWS CLI responses are usually in JSON format.

Use `jq` to filter and extract useful information.

## Example
```bash
aws ec2 describe-instances | jq '.Reservations[].Instances[].InstanceId'
```

This extracts only EC2 Instance IDs from the JSON output.

---

# Output Redirection

Store script output into a file:

```bash
./resource-tracker.sh > output.txt
```

Used for report generation and logging.

---

# Cron Job Automation

Automate script execution at scheduled intervals.

## Open Crontab
```bash
crontab -e
```

## Example
```bash
0 * * * * /home/ubuntu/resource-tracker.sh
```

Runs the script every hour automatically.

---

# DevOps Relevance

This project demonstrates:

- AWS CLI usage
- Shell scripting automation
- Cloud resource monitoring
- Cost optimization
- Cron job scheduling
- JSON parsing using jq

---

# Key Takeaways

- Learned AWS CLI basics
- Understood resource tracking concepts
- Practiced shell scripting automation
- Learned output redirection
- Understood cron job scheduling
- Explored JSON parsing with jq

---

# Future Enhancements

- Email notifications
- Slack alerts
- CloudWatch integration
- Automated cleanup scripts
- Resource usage dashboards
