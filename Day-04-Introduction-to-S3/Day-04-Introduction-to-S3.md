# Day 4 - Introduction to S3 - Quick Notes

**Date:** 12/16/2025 | **Time:** 4 hours | **Status:** ✅ Complete 

---

## 🎯 Today's Goals

- [X] Understanding what is S3 (Simple Storage Service)
- [X] Understanding the concept of buckets and objects
- [X] Overview of S3 storage classes
- [X] Understanding S3 Bucket naming convention

---

## 📚 What I Learned (5-Minute Summary)

**Main Topic:** Amazon S3 (Simple Storage Service)

**Key Takeaways:**
1. S3 is object-based storage designed for durability and scalability, not traditional file system or operating systems
2. Everything in S3 lives inside a bucket, and every file is stored is an object with metadata and permissions attached
3. Storage classes exist to balance cost and access needs - choosing the right one matters just as much as storing the data itself.

**New Terms:**
- **Bucket:** A globally unique container that holds objects in S3 and defines configuration, permissions, and region
- **Object:** A file stored in S3 that includes data, metadata, and unique key (name).

---

## 🛠️ What I Built

**Exercise/Project:** Static Website Hosted on Amazon S3

![S3 Bucket diagram](./screenshots/S3-bucket.png)


**What I did:**
- Created an S3 bucket following AWS naming conventions
- Uploaded static website files (HTML and tex objects)
- Configured bucket permissions and object ownership
- Disabled public access blocks intentionally and securely
- Made objects publicly readable to host a static website
- Verified access via the S3 public URl




***

***


***


**Result:**
I successgully hosted a static website using Amazon S3 and accessed it publicly through a browser.  This confirmed my understanding of buckets, objects, permissions, and how S3 can be used for real-world workloads beyond simple file storage. 

**Screenshots:** 

### 1. Click on Create bucket
![Step 1 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/cb9f2aab-35a1-4dd3-bf3f-58d22856514b/86be1829-3116-4cb6-a0a4-d29d96a04eb1.png?crop=focalpoint&fit=crop&fp-x=0.5225&fp-y=0.2523&fp-z=2.5207&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=454&mark-y=349&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yOTMmaD04MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 2. Naming Bucker"
![Step 2 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/fbbc4897-bbc4-4966-94fb-a5b5cb2078ee/d91cf665-ac60-46f4-801d-2716f19f0f3b.png?crop=focalpoint&fit=crop&fp-x=0.3378&fp-y=0.4633&fp-z=1.0863&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=36&mark-y=372&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz04MDkmaD0zNSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 3. Click on Create bucket
![Step 3 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/a461f043-4885-4c10-a29b-75e2f8c475ed/bec7aac9-f9c9-42a7-aae3-c89354ab56d8.png?crop=focalpoint&fit=crop&fp-x=0.9281&fp-y=0.9059&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=623&mark-y=421&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz00NjQmaD0xMjkmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 4. Click on shannon-aws-learning-2025
![Step 4 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/2aebaeb9-089e-4183-91c8-26f9e15d331e/11a0f47f-90d1-432a-b640-351b331cdd22.png?crop=focalpoint&fit=crop&fp-x=0.1283&fp-y=0.4990&fp-z=2.3460&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=183&mark-y=366&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zNTUmaD00NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 5. Click on Upload
![Step 5 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/d6c61451-d0ec-4485-986e-00e3f533f35f/8727dcf9-acb5-4f7c-a00b-ddade91384df.png?crop=focalpoint&fit=crop&fp-x=0.9322&fp-y=0.2658&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=820&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yODMmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 6. Click on Add files
![Step 6 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/e3a4c6f4-2d03-4354-911e-c3f90db2f499/71e0aa3b-30a7-4491-850a-1348f4aaf713.png?crop=focalpoint&fit=crop&fp-x=0.8432&fp-y=0.3185&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=518&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yNjImaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 7. Select a file from upload menu
![Step 7 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/64abe099-8ddb-4afe-b65e-35b7afe05bf2/5af206aa-87c7-45d6-80d8-793d3121d74e.png?crop=focalpoint&fit=crop&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n)


### 8. Click on Upload
![Step 8 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/fdd0bb53-b58f-4363-97bf-40462fa56523/40fa458d-66a0-4d85-9d64-76db2c3494f9.png?crop=focalpoint&fit=crop&fp-x=0.9429&fp-y=0.9286&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=765&mark-y=492&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zMjImaD0xMjkmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 9. Click on Close
![Step 9 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/6cc6e1f9-0e08-4333-b676-8feabf43b22f/3bfb4998-f52a-480a-b4ba-bba0c9bb92f8.png?crop=focalpoint&fit=crop&fp-x=0.9577&fp-y=0.2048&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=947&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yMDgmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 10. Click on text-for-s3-bucket.txt
![Step 10 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/49dc867f-1021-4913-819d-96810cc94385/7e9fa5f6-b7a0-4b35-b18b-3126c9cb2cda.png?crop=focalpoint&fit=crop&fp-x=0.1303&fp-y=0.5403&fp-z=2.5122&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=245&mark-y=364&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yOTYmaD01MSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 11. Click on URL for text file
![Step 11 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/35ba6d37-15ef-402e-912f-01ec4297a62f/85e6dd81-5a6c-45a8-ac34-6f452878febf.png?crop=focalpoint&fit=crop&fp-x=0.7139&fp-y=0.5165&fp-z=2.0942&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=119&mark-y=369&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz05NjImaD00MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 12. Click on shannon-aws-learning-2025
![Step 12 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/52d63ce8-9970-44ba-8ab4-e5d664e66b29/dc17ce28-a7a3-48ed-965c-03d1ea35fbd7.png?crop=focalpoint&fit=crop&fp-x=0.2236&fp-y=0.0755&fp-z=2.3460&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=422&mark-y=112&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zNTUmaD01MyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 13. Click on Permissions
![Step 13 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/98734b7b-8ecd-4896-87d2-51156287ffda/3fbf2a81-9f1c-4baf-9d29-ddddd4354bb8.png?crop=focalpoint&fit=crop&fp-x=0.4731&fp-y=0.1944&fp-z=2.6137&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=470&mark-y=335&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yNTkmaD0xMTAmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 14. Click on Edit
![Step 14 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/529070c6-567f-42ec-9a90-e4032ba79c5f/79425f30-1e36-4c6f-bd10-664dd293c492.png?crop=focalpoint&fit=crop&fp-x=0.9362&fp-y=0.4250&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=884&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xODQmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 15. Uncheck Block all public access
![Step 15 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/b4adc7c6-bfc7-420d-ab09-fb27f0812098/352b628d-c323-4860-9dd7-5275818e7c66.png?crop=focalpoint&fit=crop&fp-x=0.2243&fp-y=0.3175&fp-z=3.0786&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=570&mark-y=360&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz02MCZoPTYwJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 16. Click on Save changes
![Step 16 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/1716b17a-0db7-47af-b24e-a8af72151ea5/483cac8f-4d11-4ab4-9963-0e836636d7cf.png?crop=focalpoint&fit=crop&fp-x=0.9392&fp-y=0.6174&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=820&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zMzMmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 17. Type "confirm"
![Step 17 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/4276249d-96cb-4a29-a715-d7febd613f45/5711148c-c18b-4602-ada7-9f2304a9b042.png?crop=focalpoint&fit=crop&fp-x=0.5003&fp-y=0.5564&fp-z=1.4674&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=264&mark-y=366&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz02NzImaD00NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 18. Click on Confirm
![Step 18 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/9c0b7d40-a942-4ca9-ade0-7d216c3388c6/66f8fa9f-55e0-4c24-a76f-3c45a0e81714.png?crop=focalpoint&fit=crop&fp-x=0.6548&fp-y=0.6194&fp-z=2.6940&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=485&mark-y=346&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yMzAmaD04NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 19. Click on Edit
![Step 19 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/394f5a5f-85e1-47b4-b66b-0290ae00f09d/0329eab9-934c-4eeb-a9aa-c68477280bab.png?crop=focalpoint&fit=crop&fp-x=0.9362&fp-y=0.4840&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=884&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xODQmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 20. Click on Object Ownership
![Step 20 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/18f6ff1d-7127-4140-b1a6-c95657a05410/419208d7-39d2-40a4-ac18-fe8af38317d9.png?crop=focalpoint&fit=crop&fp-x=0.4671&fp-y=0.3402&fp-z=1.2759&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=216&mark-y=282&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz03NjgmaD0xMTMmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 21. Check I acknowledge that ACLs will be restored.
![Step 21 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/af2cbde3-404d-4a19-876b-b69eed7afb9e/e064cb6d-e7ea-4494-89cf-32f90daf0b30.png?crop=focalpoint&fit=crop&fp-x=0.2525&fp-y=0.5915&fp-z=3.0786&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=570&mark-y=360&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz02MCZoPTYwJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 22. Click on Save changes
![Step 22 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/d43032fe-da72-4f17-9ddc-428941dc6d28/6e9e706c-572a-4718-9fd8-3c69e6d8d4bd.png?crop=focalpoint&fit=crop&fp-x=0.9291&fp-y=0.9090&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=633&mark-y=431&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz00NTUmaD0xMjkmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 23. Click on Objects
![Step 23 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/1f709394-fa04-41a9-91e1-c9849c14fe54/ff9df670-53a7-4cd6-a243-d72ada00a077.png?crop=focalpoint&fit=crop&fp-x=0.2384&fp-y=0.2523&fp-z=2.7744&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=499&mark-y=332&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yMDEmaD0xMTYmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 24. Click on index.html
![Step 24 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/c87adf7c-c650-4e9c-bae3-97e49ba031f6/55e36b13-6eef-4dc5-9f4a-b93c1662013e.png?crop=focalpoint&fit=crop&fp-x=0.2955&fp-y=0.5207&fp-z=2.8487&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=513&mark-y=361&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xNzQmaD01NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 25. Click on Object actions
![Step 25 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/eff12cab-f85d-4ba1-96be-c2c2bb330f21/7ddf5db7-9001-4b53-8f20-6d03a86cbc31.png?crop=focalpoint&fit=crop&fp-x=0.9201&fp-y=0.1386&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=721&mark-y=269&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zOTcmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 26. Click on Make public using ACL
![Step 26 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/0576e096-75b2-4fc1-86e4-0ab3bb4ae71a/c01ff353-eeb2-43fe-9067-e34de3980312.png?crop=focalpoint&fit=crop&fp-x=0.8942&fp-y=0.5491&fp-z=2.9653&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=536&mark-y=347&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz01NzYmaD04NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 27. Click on Make public
![Step 27 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/16953bbe-f95d-4075-ac34-c1d171d1ecfd/8c4cf7c1-60c1-4bb5-a485-e6c2788339e9.png?crop=focalpoint&fit=crop&fp-x=0.9422&fp-y=0.4767&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=841&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zMTImaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 28. Click on Close
![Step 28 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/5abb0a1b-3840-43c1-8d7a-99489efbf924/b6f7012e-ca7d-4f5c-9ad6-b4114940bc9b.png?crop=focalpoint&fit=crop&fp-x=0.9577&fp-y=0.2048&fp-z=2.9294&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=947&mark-y=342&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yMDgmaD05NCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 29. Right click on https://shannon-aws-learning-2025.s3.us-east-1.amazonaws.com/index.html
![Step 29 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/50f41de0-b84a-4209-a12f-52cf5aa086e6/4306d8f2-0286-4b75-9e80-f5858e5c4446.png?crop=focalpoint&fit=crop&fp-x=0.6904&fp-y=0.5165&fp-z=2.0942&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=178&mark-y=369&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz04NDQmaD00MiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 30. Click on Hello From S3
![Step 30 screenshot](https://images.tango.us/workflows/1c315f2b-5c84-42ca-907f-88f03d430450/steps/17146c8e-1b51-4874-a759-18b06a625194/7348f15e-9a8e-46db-9e74-f3a5f1f345d8.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.0408&fp-z=1.0027&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=2&mark-y=14&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xMTk3Jmg9MzYmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)

<br/>

---

## 💡 Key Learning

**One thing I'll remember from today:**
S3 is simple by design, but access control is powerful - storage without intentional permissions ie either useless or dangerous.

**How I'll use it:**
I'll use S3 as the backbone for static sites, logs, backups, and future data pipelines, always choosing storage classed and permissions deliberatley instead of defaulting blindly.

---

## 🐛 Problems Faced

**Problem:** 
Understanding why objects weren't publicly accessible even after upload

**Solution:** 
I learned that S3 blocks public access by default. I had to intentionally update bucket permission, object ownership, and ACL settings to allow public access.

**Lesson:** 
AWS defaults prioritie security - accessibility is always something you must explicitly allow.

---

## 💰 AWS Resources

**Created Today:**
- S3 Bucket - Status: Active
- Static Website Objects - Status: Publicly Accessible

**Cleanup Status:**
- [X] All resources stopped/terminated
- [X] Billing checked: $0

---

## 📅 Tomorrow

**Focus:** Connecting EC2 and S3

**To-Do:**
- [ ] Create an IAM roles for EC2
- [ ] Understand how applications authenticate to AWS services
- [ ] Undersand why IAM roles are better than access keys for EC2

**Questions to Answer:**
- When should S3 not be used?
- How does S3 fit into production cloud architecture

---

## ✅ Quick Check

- [X] Learned something new
- [X] Built something working
- [X] Documented progress
- [X] Cleaned up AWS resources
- [X] Updated main README
- [X] Committed to GitHub

---

**Daily Win:** Hosting a live static website on S3 fully understanding why it works - not just that it workss.

**Tomorrow's Promise:** I wll treat cloud storage as architecture, not just a place to dump files.

---

**Day 4/90 Complete** ✓