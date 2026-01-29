# Day 5 — secure EC2 <-> S3 Integration with IAM Roles 

**90-Day Cloud Engineering Journey** 

**Date:** 12/22/2025<br> 
**Time Invested:** 4 hours<br> 
**Status:** Complete 

--- 

## Objective 

Implement **secure service-to-service authentication** between EC2 and S3 using IAM roles, eliminating the need for static access keys and aligning with AWS security best practices 

--- 

## Key Concepts Learned 

- EC2 instances should authenticate to AWS service **IAM roles**, not access keys 
- IAM roles provide **temporary, automatically rotated credentials** 
- Instance profiles allow EC2 to **assume permissions dynamically** 
- Role-based access is **more secure, scalable, and production-ready** 


Key Definitions: 
- **IAM Roles:** A permission set assumed temporarily by AWS services 
- **Instance Profile:** The mechanism that attaches a role to an EC2 instance 

--- 

## Deliverable 


**Secure EC2-to-S3 Access:** 
- Created an IAM role scoped specifically for EC2 
- Attached a least-privilege policy granting controlled S# access 
- Associated the role with an EC2 instance via an instance profile 
- Verified S3 access from EC2 **without storing credentials** 
 

**Commands Used:** 
```bash 
# Most important commands from today 
aws s3 ls 
aws s3 cp 
``` 

## Result:<br> 
The EC2 instance accessed S3 successfully using AWS-managed temporary credentials, confirming secure authentication with no credential exposure. 

--- 

## Engineering Insight 
If credentials exist on a server, they will eventually be leaked. <br> 
IAM roles eliminated this risk entirely by shifting authentication responsibility to AWS. 

--- 
 

## Problem Solved 

**Challenge:**<br> 
Understanding how EC2 could access S3 without explicitly configured credentials. 

**Resolution:**<br> 
Learned how IAM roles and instance profiles work together to supply temporary credentials transparently. 

**Lesson:**<br> 
Well-designed cloud security is invisible - when done correctly, access "just works." 

--- 


## Risk & Cost Awareness 
- IAM role created and validated 
- EC2 instance used only for testing 
- Resource stopped after verification 
- Billing checked: $0 
- No credential sprawl introduced 

--- 
 

## Next Focus Area 

**Week 1 Mini Project** 
Apply IAM, EC2, and S3 together in a small user-facing application. 

--- 

 

## Daily Outcome 
- Implemented secure service authentication using IAM roles 
- Eliminated static credentials from EC2 
- Applied least-privilege access controls 
- Documentation committed to GitHub 

**Day 5 of 90 — Complete** 
 