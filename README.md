Automated Backup & Disaster Recovery Solution (RHEL 10)
Project Overview

This project demonstrates the implementation of a production-grade automated backup and disaster recovery solution on a Red Hat Enterprise Linux (RHEL 10) server hosted on AWS EC2.

The objective was to automate application backups using Bash scripting, schedule backup execution with Cron Jobs, implement structured logging, configure backup retention policies, perform disaster recovery testing through backup restoration, and securely store backups in AWS S3 for off-site disaster recovery.

Project Objectives
Automate Linux application backups using Bash scripting.
Compress backup archives using tar and gzip.
Schedule automated backups using Cron Jobs.
Implement centralized logging and error handling.
Configure backup retention policies.
Perform disaster recovery through backup restoration.
Store backup archives securely in AWS S3.
Validate successful backup creation and restoration.
Environment

Operating System: Red Hat Enterprise Linux 10

Cloud Platform: AWS EC2

Instance Type: t2.micro

Package Manager: DNF

Cloud Storage: Amazon S3

Automation: Bash Shell Script & Cron

Project Architecture
                     Linux Application
                            │
                            ▼
                 Bash Backup Script
                            │
          ┌─────────────────┼─────────────────┐
          │                 │                 │
          ▼                 ▼                 ▼
   Create Archive      Write Logs      Verify Backup
          │
          ▼
   Compressed tar.gz
          │
          ▼
 Backup Directory (/backup)
          │
          ▼
    Backup Retention Policy
          │
          ▼
      AWS S3 Bucket
          │
          ▼
 Disaster Recovery Restore
Tasks Performed

Phase 1
Server Preparation

Updated Linux packages
Configured hostname
Installed required utilities
Verified environment

Phase 2
Created Sample Production Application

Created application directory
Added configuration files
Added log files
Created uploads directory
Created sample database backup

Phase 3
Backup Repository Configuration

Created backup directory
Configured permissions
Verified storage availability
Generated timestamp-based naming

Phase 4
Manual Backup

Created a compressed backup archive
Verified archive integrity
Listed archive contents
Compared backup sizes

Phase 5
Backup Automation

Developed Bash backup script
Used variables for reusable code
Generated timestamp-based backups
Automated archive creation

Phase 6
Logging & Error Handling

Created centralized log file
Implemented success and failure logging
Added exit status validation
Added backup statistics
Improved script readability

Phase 7
Cron Job Automation

Configured Cron service
Scheduled automated backups
Verified Cron execution
Validated scheduled backup creation

Phase 8
Disaster Recovery

Simulated application failure
Restored application from backup
Verified restored files
Validated recovery process

Phase 9
Backup Retention Policy

Implemented automatic cleanup
Deleted expired backups
Configured retention period
Logged cleanup activities

Phase 10
AWS S3 Integration

Installed AWS CLI
Configured AWS authentication
Uploaded backup archives to Amazon S3
Verified cloud backup availability
Integrated S3 upload into backup automation

Linux Commands Used
tar
gzip
find
cron
crontab
date
tee
chmod
mkdir
touch
rm
cp
mv
du
df
tree
aws
aws s3 cp
aws s3 ls
aws configure
aws sts get-caller-identity
systemctl
journalctl
hostname
whoami

Key Skills Demonstrated
Linux Administration
Bash Shell Scripting
Backup Automation
Disaster Recovery
Cron Job Scheduling
AWS S3 Integration
AWS CLI
Log Management
Error Handling
Linux File Management
Backup Retention Strategy
Shell Script Debugging
Process Automation
Production Operations
Learning Outcomes

Through this project, I gained hands-on experience in designing and implementing an automated backup and disaster recovery solution using Linux and AWS. I learned how to automate repetitive administrative tasks using Bash scripting, schedule jobs with Cron, maintain structured logs, implement backup retention strategies, perform disaster recovery through restoration testing, and securely store backups in Amazon S3. This project strengthened my understanding of Linux automation, operational reliability, and production backup best practices.

Future Improvements
Incremental Backups
Differential Backups
Backup Encryption using GPG
Email Notifications for Backup Status
Slack Notifications
AWS SNS Integration
Cross-Region S3 Replication
Backup Monitoring with CloudWatch
Backup Validation using Checksums
Multi-Server Backup Automation using Ansible

Author
Saurabh Singh

Learning DevOps through hands-on projects.
