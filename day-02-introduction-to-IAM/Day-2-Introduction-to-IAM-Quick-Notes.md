# Day 2 - Introduction to IAM - Quick Notes

**Date:** 12/12/2025 | **Time:** 5 hours | **Status:** ✅ Complete

---

## 🎯 Today's Goals

- [X] IAM overview: Users, Groups, Policies, Roles
- [X] Understanding AWS permission model
- [X] Principle of least privilege

---

## 📚 What I Learned (5-Minute Summary)

**Main Topic:** AWS Identify and Access Management (IAM)

**Key Takeaways:**
1. A single IAM user can belong to multiple groups - and that's the cleanest way to manage permission
2. IAM is all about controlling "who can do what" inside AWS. Users, Groups, Policies, and Roles all connect to enforce secure access
3. The principle of least privilege is non-negotiable - always give the minimum permissions a person or service needs, nothing extra

**New Terms:**
- **IAM User:** A person or application that interacts with AWS using a username/password or access keys
- **IAM Role:** A temporary identity with specific permissions that a user or service can assume when needed

---

## 🛠️ What I Built

**Exercise/Project:** Added IAM user and groups

IAM Architecture Diagram
![IAM Architecture Diagram](./screenshot/IAM.png)


**What I did:**
# [Create IAM Users with EC2 Access](https://app.tango.us/app/workflow/8730f5e4-6374-41bd-b30f-ee8f5480d130?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)

***

## # [Console Home | Console Home | us-east-1](https://us-east-1.console.aws.amazon.com/console/home?nc2=h_si&region=us-east-1&src=header-signin#)

### 1. Click on IAM
![Step 1 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/86039de0-e045-415d-9bb6-09d9551a96e9/4d79c597-b3a6-4fc1-8582-e87d7da3e992.png?crop=focalpoint&fit=crop&fp-x=0.1839&fp-y=0.2111&fp-z=3.0815&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=567&mark-y=325&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02NyZoPTUzJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 2. Click on Users
![Step 2 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/a750c36c-2a57-4bdd-b123-51ed133c49d5/d87dfa02-bd57-4152-b7a2-f97f3470ccac.png?crop=focalpoint&fit=crop&fp-x=0.0248&fp-y=0.3369&fp-z=3.0815&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=48&mark-y=325&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz04NyZoPTUzJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 3. Click on Create user
![Step 3 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/1720691f-5426-49e8-a06a-1be7c40ac705/8773aeb2-04df-49a9-8fe8-7bf43f4fd33e.png?crop=focalpoint&fit=crop&fp-x=0.9465&fp-y=0.4099&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=886&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yNDYmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 4. Click on User name
![Step 4 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/d14b8bd3-0bd5-41df-9d18-dee75cb9d705/a1a1ee61-6739-49c6-888e-d3197d85bf80.png?crop=focalpoint&fit=crop&fp-x=0.4539&fp-y=0.2639&fp-z=1.2942&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=233&mark-y=223&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MzQmaD0zNCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 5. Type "Testuser1"
![Step 5 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/598f34a1-1eb5-4e3b-8963-5019d86a70cd/35c045f9-8a1e-4884-a350-c6967254417d.png?crop=focalpoint&fit=crop&fp-x=0.4539&fp-y=0.2639&fp-z=1.2942&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=233&mark-y=223&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03MzQmaD0zNCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 6. Click on Next
![Step 6 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/4c52e6f6-c3c6-4551-97a8-a70596a65cab/f63eacc0-950e-46e6-94a1-7fdc94aa2826.png?crop=focalpoint&fit=crop&fp-x=0.9179&fp-y=0.4909&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=827&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xNjAmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 7. Check on
![Step 7 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/10af5b5d-931f-4cfa-9c20-d6bdad2ba4a2/b3cc710b-0eb2-456d-88a9-4093ca98d3bf.png?crop=focalpoint&fit=crop&fp-x=0.2310&fp-y=0.5357&fp-z=3.1019&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=576&mark-y=327&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00OSZoPTQ5JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 8. Click on Next
![Step 8 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/8b7fd570-3110-49ed-8176-eefc82c4c6c5/4b933337-f0f8-407b-b44d-e49d699100e5.png?crop=focalpoint&fit=crop&fp-x=0.9179&fp-y=0.6647&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=827&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xNjAmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 9. Click on Create user
![Step 9 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/c78fb5da-6205-4694-956c-46a2f63cd5bb/8f838cc7-6f1d-43a1-b33b-2f156c360d91.png?crop=focalpoint&fit=crop&fp-x=0.9059&fp-y=0.6658&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=741&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yNDYmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 10. Click on Testuser1
![Step 10 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/26c4be7e-867b-4ddb-a98c-fae250b6d059/ba1a356d-f7ff-481f-af72-88895ecde8b9.png?crop=focalpoint&fit=crop&fp-x=0.2162&fp-y=0.7495&fp-z=2.9605&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=533&mark-y=326&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xMzQmaD01MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 11. Click on Add permissions
![Step 11 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/e8be4080-52b4-4484-8cfe-467be1bf0a6d/ad47ce96-c7e5-4877-8e2c-ac8eb37e0945.png?crop=focalpoint&fit=crop&fp-x=0.9205&fp-y=0.5341&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=740&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zNTMmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 12. Click on Add permissions
![Step 12 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/afd45ef9-1f89-4ad0-ae36-803e0d513c0e/3eb42884-bf0b-4c57-810a-a0068c61d937.png?crop=focalpoint&fit=crop&fp-x=0.9185&fp-y=0.5674&fp-z=2.9978&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=726&mark-y=316&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zNjImaD03MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 13. Select Attach policies directly
![Step 13 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/02495cbe-dc3b-4895-bb1a-e389b31bfe32/1243ec98-76cb-4cc8-89ea-920c3cdb99a8.png?crop=focalpoint&fit=crop&fp-x=0.7206&fp-y=0.2559&fp-z=3.1019&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=576&mark-y=327&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00OSZoPTQ5JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 14. Type "EC2"
![Step 14 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/09938693-9b58-4e37-829a-5c473dbd5154/127400c0-564d-4dbc-902c-e3d101c5923c.png?crop=focalpoint&fit=crop&fp-x=0.3576&fp-y=0.4462&fp-z=1.5152&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=273&mark-y=332&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02NTUmaD00MCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 15. Check on
![Step 15 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/33241a9d-2fff-475c-bba2-0422f231d84d/092dc546-1235-4950-a7d5-f3b8cd1f34ca.png?crop=focalpoint&fit=crop&fp-x=0.1908&fp-y=0.8070&fp-z=3.1937&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=575&mark-y=326&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01MCZoPTUwJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 16. Click on Next
![Step 16 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/a866ebc8-9d56-43c4-b6f3-72a093e94632/4842c092-77c2-4798-92a5-5cda652e9485.png?crop=focalpoint&fit=crop&fp-x=0.9585&fp-y=0.9158&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=893&mark-y=415&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yMTYmaD0xMDImZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)

### 17. Click on Add permissions
![Step 17 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/e00972c4-0928-4560-9244-6425bf7d24f2/04c9d2b0-c31b-4294-8237-1f2f12f6c7e4.png?crop=focalpoint&fit=crop&fp-x=0.9369&fp-y=0.4733&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=818&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zMTQmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 18. Click on Security credentials
![Step 18 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/351d40f1-ee0b-45c2-a707-ca4a9de1c6c4/5de0dca7-5d9b-4aca-ae58-b35d6b000a42.png?crop=focalpoint&fit=crop&fp-x=0.3926&fp-y=0.3963&fp-z=2.5065&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=451&mark-y=309&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yOTgmaD04NSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 19. Click on Enable console access
![Step 19 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/59638510-adba-43c9-9d49-8121f87e5aed/cd232bf2-9d08-4f9b-8f9c-ef6ab2908cb6.png?crop=focalpoint&fit=crop&fp-x=0.9162&fp-y=0.4595&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=710&mark-y=314&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zODImaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 20. Select Custom password
![Step 20 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/cf5bf1f4-74ce-4d35-9221-2cc552cd0e91/e8481b48-2a95-405d-972d-6ba91f893683.png?crop=focalpoint&fit=crop&fp-x=0.3475&fp-y=0.4291&fp-z=3.1019&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=576&mark-y=327&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00OSZoPTQ5JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 21. Paste input
![Step 21 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/cc53b97b-511e-4601-88ee-f3f80747369a/5e91a1e2-0568-48a2-9bd0-8f693a44ecf7.png?crop=focalpoint&fit=crop&fp-x=0.4961&fp-y=0.4574&fp-z=1.6993&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=306&mark-y=329&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01ODgmaD00NSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 22. Click on Enable console access
![Step 22 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/495bf77c-1700-4983-9990-e4416528d15a/9e0808c8-e141-49df-aded-a2911806d98e.png?crop=focalpoint&fit=crop&fp-x=0.5977&fp-y=0.6887&fp-z=2.4565&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=442&mark-y=320&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0zMTYmaD02MyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 23. Click on Close
![Step 23 screenshot](https://images.tango.us/workflows/8730f5e4-6374-41bd-b30f-ee8f5480d130/steps/60c3c8e8-ba16-4002-a0d6-66e2d28c6587/1cb367c7-4530-4de6-b47b-b56f5e0c5010.png?crop=focalpoint&fit=crop&fp-x=0.6313&fp-y=0.6610&fp-z=2.8781&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=518&mark-y=315&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xNjQmaD03MyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

<br/>

***

# [Create a Finance Dept User Group in IAM](https://app.tango.us/app/workflow/5bb6cc2b-2999-480c-94ad-6c4e1331f27b?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)


***



## # [Console Home | Console Home | us-east-1](https://us-east-1.console.aws.amazon.com/console/home?region=us-east-1)

### 1. Type "IAM"
![Step 1 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/3c9629c6-d506-4ea0-9712-c9a87a516209/de8a2c28-2d65-41a9-971b-68e239919d4a.png?crop=focalpoint&fit=crop&fp-x=0.2100&fp-y=0.0264&fp-z=1.6683&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=121&mark-y=10&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01OTkmaD00MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 2. Click on IAM
![Step 2 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/8e5a6a6b-44c5-4677-866e-3aea891b695e/a8796488-2bee-45fd-9ce1-55a0aa57c087.png?crop=focalpoint&fit=crop&fp-x=0.2374&fp-y=0.1261&fp-z=3.0664&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=563&mark-y=244&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03NSZoPTU2JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 3. Click on User groups
![Step 3 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/7d99312c-48fe-4eea-81d3-d5ac0bf7958e/221ae5e5-6cfb-4745-a3ad-b8be11449a62.png?crop=focalpoint&fit=crop&fp-x=0.0361&fp-y=0.3108&fp-z=2.8911&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=45&mark-y=327&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0xNTkmaD01MCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 4. Click on Create group
![Step 4 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/3bdf10d4-4f35-43f5-916a-7795f0156cf9/7cb9701d-1811-4147-83d7-a55ae1415a7d.png?crop=focalpoint&fit=crop&fp-x=0.9438&fp-y=0.1135&fp-z=2.9740&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=865&mark-y=199&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz0yNzAmaD03NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 5. Type "Finance Dept"
![Step 5 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/26cc9353-abf8-459f-9f6e-4c1675baf00c/1ae1db49-40f4-471a-a187-a87d195cf4f0.png?crop=focalpoint&fit=crop&fp-x=0.4391&fp-y=0.2447&fp-z=1.2128&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=216&mark-y=193&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03NjcmaD0zMiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 6. Type "Bill"
![Step 6 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/4b5f2ee8-95bf-4a02-87b1-0fdaf6776f63/0a89ec1f-5dea-4cf4-b806-e89d597ef164.png?crop=focalpoint&fit=crop&fp-x=0.3561&fp-y=0.6764&fp-z=1.5123&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=272&mark-y=339&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz02NTYmaD00MCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 7. Check on
![Step 7 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/edc5aa53-d039-4be9-8232-8207ec134292/20331092-abc6-409a-af51-430a7cca27d6.png?crop=focalpoint&fit=crop&fp-x=0.1892&fp-y=0.7511&fp-z=3.1937&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=575&mark-y=326&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01MCZoPTUwJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 8. Check on
![Step 8 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/7b3cfa56-4def-4660-9560-cf5248340cf8/0cb2c563-b97b-40e1-8ba1-8f3fe8c4dcc8.png?crop=focalpoint&fit=crop&fp-x=0.1892&fp-y=0.8582&fp-z=3.1937&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=575&mark-y=359&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz01MCZoPTUwJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 9. Check on
![Step 9 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/b5c27933-2d42-4624-a731-9a91bbd08c12/6068f99c-0a86-436b-a3cd-c0973b0493e3.png?crop=focalpoint&fit=crop&fp-x=0.1892&fp-y=0.5261&fp-z=3.1019&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=576&mark-y=327&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00OSZoPTQ5JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)

### 10. Click on Create user group
![Step 10 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/2fa511fa-7182-4d88-9c55-e878dd3ff88e/e2ee17ae-3b9a-4919-bcf7-6be5c61a69fa.png?crop=focalpoint&fit=crop&fp-x=0.9351&fp-y=0.9163&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=665&mark-y=417&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00NDcmaD0xMDImZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)

### 11. Type "Finance-Dept"
![Step 11 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/74c00ebc-1c0c-4f62-b67c-fdc8d5ea2688/5342464f-6dce-4ebe-930d-5af9b47ea207.png?crop=focalpoint&fit=crop&fp-x=0.4391&fp-y=0.1828&fp-z=1.2128&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=216&mark-y=140&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz03NjcmaD0zMiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)

### 12. Click on Create user group
![Step 12 screenshot](https://images.tango.us/workflows/5bb6cc2b-2999-480c-94ad-6c4e1331f27b/steps/2b99fa7b-7053-4ede-8efd-8fd7c4b5ee01/5f1b5926-def5-4d42-b266-ef3fc79a4dbe.png?crop=focalpoint&fit=crop&fp-x=0.9351&fp-y=0.9163&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=665&mark-y=417&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTYlMkNGRjc0NDImdz00NDcmaD0xMDImZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)

<br/>

***

**Commands Used:**
```bash
# No CLI commands used today
```

**Result:** I created users and groups, assigning each user to a group with the exact policies they needed. One user had full EC2 access, while the other was limited to read-only permissions.


**Screenshots:** 

User with read-only permission for the EC2

![User with read-only permission for the EC2](./screenshot/EC2-read-only-permission.png)
---

## 💡 Key Learning

**One thing I'll remember from today:**
Never use the root account for everyday tasks - IAM exists for a reason, and using the right identities keeps my environment secure and manageable.

**How I'll use it:**
By creating dedicated users, groups, and roles for every task going forward. No more "quick fixes' using root. Everything I build from here on will follow least privilege and clean permission boundaries.

---

## 🐛 Problems Faced

**Problem:** One of the users I created had full EC2 access on paper, but still couldn't connect to the instance using EC2 Instance Connect. The permission looked right, but weren't complete.
Original Permission(./screenshot/permission-before.png)

**Solution:** I reviewed the IAM policy and discovered the missing EC2 Instance Connect permission. After attaching the correct policy, the user could connect successfully.
Adding the correct permission(./screenshot/permission-after.png)

**Lesson:** If something isn't working in AWS, always check the permission policy first - IAM will expose you quick.

---

## 💰 AWS Resources

**Created Today:**
- IAM Users
- IAM Groups
- EC2 Instance - Status: Stopped

**Cleanup Status:**
- [X] All resources stopped/terminated
- [x] Billing checked: $0

---

## 📅 Tomorrow

**Focus:** EC2 Instance

**To-Do:**
- [ ] Understand what is EC2 (Elastic Compute Cloud)
- [ ] Instance types overview
- [ ] Amazon Machine Images (AMIs)
- [ ] Security Groups Basics
- [ ] SSH Key pairs


---

## ✅ Quick Check

- [X] Learned something new
- [X] Built something working
- [X] Documented progress
- [X] Cleaned up AWS resources
- [X] Updated main README
- [X] Committed to GitHub

---

**Daily Win:** 
Creating users and groups confidently - and fixing a permission issue on my own without panicking

**Tomorrow's Promise:** 
I will dive into EC2 with intention and clarity, and I'll build only what I understand.

---

**Day 2/90 Complete** ✓


