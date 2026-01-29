# Day 3 — EC2 Compute Fundamentals
**90-Day Cloud Engineering Journey**

**Date:** 12/15/2025<br>
**Time Invested:**  6 hours<br>
**Status:**  Complete<br>

---

## Objective

Provision and operate an **EC2 instance** end-to-end, focusing on compute selection, secure access, networking, and service lifecycle management.<br>
This day emphasized **understanding why instance fail to connect,** not just launching them.

---

## Core Concepts Applied

- EC2 provides **full control over compute,** including OS, services, and networking
- Instance type selection directly impacts **cost and performance**
- AMIs define the **baseline operating environment**
- Security Groups and SSH key pairs are **mandatory gatekeepers**
- Compute is unusable without **aligned networking and permissions**

---

## Deliverable

**EC2 Web Server Deployment:**
- Launched an EC2 instance using an Amazon Linux AMI
- Selected an appropriate instance type for lightweight web hosting
- Configured Security Groups rules to allow HTTP and SSH access
- Generated and secured an SSH key pair
- Connected via SSH and installed Apache Web Server
- Verified application availability via public IPv4 address

**Operational Validation:**
- Started, stopped, enabled, and disabled Apache
- Practiced EC2 instance lifecycle management
- Confirmed service availability through browser testing

---

## Engineering Insight

An EC2 instance is not usable by default.<br>
**Compute, networking, security groups, and key permissions must align** before anything works - and missing any one of them will look like a "broken server."

---

## Problem Solved
**Issue:**<br>
SSH connection failed despite correct inbound rules.

**Diagnosis:**<br>
AWS configuration was correct. The issue was **local SSH key file permissions.**

**Resolution:**<br>
Updated the key pair file to read-only for the owner, restoring SSH access.

**Lesson:**<br>
EC2 troubleshooting requires checking **both AWS-side configuration and local system permissions.**

---

## Risk & Cost Awareness

- EC2 instance used only for validation
- Apache service stopped after testing
- Instance stopped after completion
- Billing verified: $0
- No idle resources left running

---

## Next Focus Area

Amazon S3
- Object storage fundamentals
- Buckets vs objects
- Storage classes and durability
- When to use S3 instead of EC2 storage

---

## Daily Outcome

- Provisioned and secure AWS compute
- Deployed and validated a live web service
- Resolved a real-world SSH access issue independently
- Practiced service and instance lifecycle management
- Documentation committed to GitHub

**Day 3 of 90 — Complete**


