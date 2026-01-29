# Day 4 — Amazon S3 (Object Storage Fundamentals)
**90-Day Cloud Engineering Journey**

**Date:** 12/16/2025<br>
**Time Invested:** 4 hours<br>
**Status:**  Complete<br>

---

## Objective

Understand **Amazon S3 as a core cloud storage service,** including when to use it, how data is organized, and why it is foundational to scalable, durable architectures.

---

## Key Concepts Learned

- S3 is **object storage,** not block file storage
- Data is stored as **objects inside buckets,** not attached to compute
- S3 is designed for **high durability, availability, and scale**
- Storage classes allow **cost optimization** based on access patterns
- Access to S3 is controlled through **IAM and bucket policies** 

Core Definitions:
- **Buckets:** Globally unique container for objects
- **Objects:** Data + metadata stored in S3
- **Storage Classes:** Different cost tiers based on access frequency

---

## Deliverable

**S3 Fundamentals Applied:**
- Created and configured an S3 bucket
- Uploaded and managed objects
- Reviewed storage class options and use cases
- Applied naming rules and access considerations

**AWS Resources:**
- S3 Bucket (used for learning, not production data)

---

## Engineering Insight

S3 decouples **storage from compute,** which fundamentally changes how systems scale.<br>
Unlike EC2 storage, S3 is built for **durability first,** making it ideal for backups, static assets, logs, and data lakes.

---

## Risk & Cost Awareness

- Resources created: Yes (S3 bucket)
- Billing checked: Yes
- Cleanup performed: Yes (no unnecessary data stored)
- No unexpected costs incurred

---

## Next Focus Area

**S3 Security & Access Control**
Understanding bucket policies, IAM permission, and public access settings in critical before using S3 in real environments.

---

## Daily Outcome

- Built a clear mental model of object storage
- Differentiated S3 from EC2-based storage
- Practiced safe, cost-aware usage
- Documentation committed to GitHub

**Day 4 of 90 — Complete**


