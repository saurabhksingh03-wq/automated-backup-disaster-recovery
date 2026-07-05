# automated-backup-disaster-recovery
Production-ready automated backup and disaster recovery solution using Bash scripting, Cron Jobs, AWS S3, logging, backup retention, and restore automation on RHEL 10.
Automated Backup & Disaster Recovery Solution
Project Overview

This project demonstrates the implementation of an automated backup and disaster recovery solution on a Red Hat Enterprise Linux (RHEL 10) server hosted on AWS EC2. The solution automates application backups using Bash scripting, schedules backups with Cron, stores backup archives with timestamp-based naming, enforces backup retention policies, and supports disaster recovery through restoration of archived data. The solution is further enhanced by integrating AWS S3 for secure off-site backup storage.

Objectives
1. Automate Linux backups using Bash.
2. Schedule backups using Cron.
3. Maintain detailed execution logs.
4. Handle backup failures gracefully.
5. Implement backup retention policies.
6. Restore applications from backup archives.
7. Store backups securely in AWS S3.

Environment
AWS EC2
Red Hat Enterprise Linux 10
Bash
Cron
AWS CLI
Amazon S3

