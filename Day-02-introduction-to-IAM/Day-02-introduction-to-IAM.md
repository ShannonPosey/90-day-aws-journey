# Day 2 — Identity & Access Management (IAM)
**90-Day Cloud Engineering Journey**

**Date:**  12/12/2025
**Time Invested:**  5 hours
**Status:**  Complete

---

## Objective

Establish secure access control in AWS by understanding and applying **IAM Fundamentals**, including users, groups, policies, and least-privilege design.
This day focused on **security-first cloud setup,** not speed.

---

## Key Concepts Learned

- IAM controls **who can do what** inside AWS
- Permissions scale cleanly through **groups**, not individual users
- **Least Privilege** is mandatory for secure, manageable cloud environments
- Roles provide **temporary permissions** and should be preferred for services and automation

**Core IAM Components:**
- **Users:** Human or application identities
- **Groups:** Permission boundaries applied at scale
- **Policies:** JSON documents defining allowed actions
- **Roles:** Temporary identities assumed when needed

---

## Deliverable

**IAM Configuration:**
- Created multiple IAM user and user groups
- Assigned permissions using **group-based policies**
- Implemented **read-only vs full-access separation** for EC2
- Enabled console access securely for designed users

Security Practice Applied
- Avoided root account usage entirely
- Followed least privileged principles for all permissions
- Validated permissions through real access testing

**AWS Resources:**
- No CLI used - work completed via AWS Console

---

## Engineering Insight

IAM is the foundation of every secure cloud environment.
If permissions are wrong, **nothing else works** - and when something breaks, IAM is often the root cause.

---

## Problem Solved
**Issue:**
A user with EC2 permission could not connect to an instance using EC2 Instance Connect.


**Diagnosis:**
Permissions appeared correct at a high level but were missing the required **EC2 Instance Connect** action.

**Resolution:**<br>
Updated the IAM policy to include the missing permission, restoring access immediately.

**Lesson:**
AWS failures are often permission-related - always inspect IAM policies before troubleshooting infrastructure.

---

## Risk & Cost Awareness

- IAM Users and Groups created
- EC2 instance used for testing (stopped after validation)
- Billing verified: $0
- No unused or running resources left active

---

## Next Focus Area

**EC2 Fundamentals**
- Instance types and AMIs
- Security Groups
- Key pairs and SSH access
- Understanding compute before scaling

---

## Daily Outcome

- Implemented secure IAM architecture
- Applied least privilege access controls
- Resolved a real-world permission issue independently
- Documentation committed to GitHub

**Day 2 of 90 — Complete**


