# aws-ebs-storage-backup-recovery
# AWS Cloud Infrastructure – EBS Storage, Backup & Recovery

## Project Overview

This project was completed as part of my Cloud Infrastructure lab. I worked with Amazon Elastic Block Store (EBS) to create and manage storage for an EC2 instance. The lab also involved creating a snapshot backup and restoring deleted data using a new EBS volume.

## Technologies Used

- Amazon Web Services (AWS)
- Amazon EC2
- Amazon Elastic Block Store (EBS)
- AWS Systems Manager Session Manager
- Linux Command Line
- Ext3 File System

## Lab Implementation

**1. EBS Volume Creation and Attachment**

Created a 1 GiB EBS volume and attached it to an existing EC2 instance in the same Availability Zone.

**2. File System Configuration**

Connected to the Linux instance using Session Manager, created an ext3 file system, and mounted the new volume under `/mnt/data-store`.

**3. Data Storage and Verification**

Created a text file on the mounted volume and verified its contents using Linux commands.

**4. Snapshot Backup**

Created an EBS snapshot to back up the volume before deleting the original text file.

**5. Data Recovery**

Created a new EBS volume from the snapshot, attached it to the EC2 instance, and mounted it under `/mnt/data-store2`.

Verified that the deleted file was available on the restored volume.

## Project Screenshots

Screenshots of the configuration, storage management, snapshot creation, and recovery process are available in the `screenshots` folder.

## What I Learned

Through this lab, I gained hands-on experience with AWS storage management, Linux file systems, EBS snapshots, and data recovery. It helped me understand how cloud storage can be managed and how snapshots can be used to recover data.
