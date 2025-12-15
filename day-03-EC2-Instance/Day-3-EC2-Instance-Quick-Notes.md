# Day 3 - EC2 Instance - Quick Notes

**Date:** 12/1/2025 | **Time:** 6 hours | **Status:** ✅ Complete

---

## 🎯 Today's Goals

- [X] Understand what is EC2 (Elastic Compute Cloud)
- [X] Instance types overview
- [X] Amazon Machine Images (AMIs)
- [X] Security Groups Basics
- [X] SSH Key pairs


---

## 📚 What I Learned (5-Minute Summary)

**Main Topic:** [Topic name]

**Key Takeaways:**
1. [Most important thing learned]
2. [Second important thing]
3. [Third important thing]

**New Terms:**
- **[Term]:** [Quick definition]
- **[Term]:** [Quick definition]

---

## 🛠️ What I Built

**Exercise/Project:** Installing Apache Web Server on EC2 Instance

EC2 Architecture Diagram(./screenshots/EC2-instance.drawio.png)

**What I did:**
- Created an EC2 instance
- SSH into the instance
- Install Apache Web server

# [Launch Apache Web Server on EC2](https://app.tango.us/app/workflow/c33871e4-79fe-4661-809c-90a3d88f6188?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)

***




## # [Console Home | Console Home | us-east-1](https://us-east-1.console.aws.amazon.com/console/home?region=us-east-1)


### 1. Type "EC2"
![Step 1 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/1aa554b8-11e0-4f8b-8672-4baff42d762c/6001b0ce-f8f6-4f24-be22-46dfb6483d0f.png?crop=focalpoint&fit=crop&fp-x=0.2586&fp-y=0.0300&fp-z=1.4969&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=134&mark-y=11&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz02NjEmaD00NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 2. Click on EC2
![Step 2 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/7ce2d8db-ebfc-4b89-a07e-8e118556288b/b8939310-8c26-4490-b4fc-2a56aaf6fa9a.png?crop=focalpoint&fit=crop&fp-x=0.2921&fp-y=0.1458&fp-z=3.0302&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=556&mark-y=298&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz04OCZoPTY4JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 3. Type "Apache web server"
![Step 3 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/30917341-ada1-4cb1-8549-bf1b71a682d2/00417140-5e69-4584-8fb2-f6cbf92bf70f.png?crop=focalpoint&fit=crop&fp-x=0.2300&fp-y=0.2894&fp-z=1.4185&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=47&mark-y=286&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz02ODkmaD00NiZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 4. Click on Create new key pair
![Step 4 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/bbec2eca-2250-42d0-92c8-a171f5b8b728/1def7e90-5322-4136-a27f-d2974c1276db.png?crop=focalpoint&fit=crop&fp-x=0.5081&fp-y=0.4802&fp-z=2.5423&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=458&mark-y=347&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0yODUmaD01NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 5. Type "apache-web-server"
![Step 5 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/37dec6fb-54a6-4c27-b1ac-7ff357f58f98/edd2770a-1fd4-429d-9683-da39cb133e50.png?crop=focalpoint&fit=crop&fp-x=0.5003&fp-y=0.3441&fp-z=1.4674&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=264&mark-y=352&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz02NzImaD00NyZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 6. Click on Create key pair
![Step 6 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/cf7c8d33-a189-4118-b0f8-99cb2dd34d61/150ba5be-49f6-4956-8aaa-1e4448ea63f1.png?crop=focalpoint&fit=crop&fp-x=0.6400&fp-y=0.8103&fp-z=2.4871&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=448&mark-y=357&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0zMDUmaD04MCZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 7. Click on Network settings
![Step 7 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/47ed8e1d-543d-4959-99d1-a393999aa9af/f4d7a447-217e-46c3-9d27-4201d5b3d279.png?crop=focalpoint&fit=crop&fp-x=0.3331&fp-y=0.5080&fp-z=1.0975&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=36&mark-y=132&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz04MDUmaD00ODgmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 8. Check Allow HTTP traffic from the internet
![Step 8 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/248ac876-7385-4343-88f9-5d65f8898da4/62028e35-1fb6-482a-a63f-55a4f63caca2.png?crop=focalpoint&fit=crop&fp-x=0.0356&fp-y=0.6817&fp-z=3.0701&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=101&mark-y=346&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz01OSZoPTU5JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 9. Click on Launch instance
![Step 9 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/23aa1b18-aa48-4044-92b4-5fb85f298c45/ed605b86-3e8a-441f-bc40-a9e216039a91.png?crop=focalpoint&fit=crop&fp-x=0.9090&fp-y=0.8371&fp-z=4.0000&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=507&mark-y=311&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz01MTMmaD0xMjkmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)


### 10. Click on Instances
![Step 10 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/47495a70-110e-457c-896c-406ce7bd3c18/423440ca-0977-4e76-bc72-2db23673a8fe.png?crop=focalpoint&fit=crop&fp-x=0.0964&fp-y=0.0782&fp-z=2.8986&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=257&mark-y=138&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xNTcmaD02NSZmaXQ9Y3JvcCZjb3JuZXItcmFkaXVzPTEw)


### 11. Click on Refresh instances
![Step 11 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/17b92287-8a17-4170-8e02-c7ad2a9cd2e9/a502342c-984c-4b8e-a0cc-4ece02768e53.png?crop=focalpoint&fit=crop&fp-x=0.5662&fp-y=0.1308&fp-z=2.9165&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=553&mark-y=240&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz05NCZoPTk0JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 12. Check on
![Step 12 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/cf422a8d-fa9d-4952-aab3-ee1cb7146578/55c94172-0d48-4676-880d-25645ac5b14e.png?crop=focalpoint&fit=crop&fp-x=0.1921&fp-y=0.2894&fp-z=3.0701&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=570&mark-y=346&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz01OSZoPTU5JmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


### 13. Click on Copy public IPv4 address to clipboard
![Step 13 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/f9c86ab1-8219-4e2a-912d-8ea4e85e1dc7/10b33597-5870-4706-a45b-2082b29fd24a.png?crop=focalpoint&fit=crop&fp-x=0.4527&fp-y=0.7385&fp-z=3.1105&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=560&mark-y=341&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz04MCZoPTcwJmZpdD1jcm9wJmNvcm5lci1yYWRpdXM9MTA%3D)


## # [18.212.207.197](http://18.212.207.197/)


### 14. Click on Hello from EC2
![Step 14 screenshot](https://images.tango.us/workflows/c33871e4-79fe-4661-809c-90a3d88f6188/steps/62be97a5-8435-4084-b622-eeacc19f0583/81416623-11ce-4753-ae05-41e24d0eeccc.png?crop=focalpoint&fit=crop&fp-x=0.5000&fp-y=0.0274&fp-z=1.0027&w=1200&border=2%2CF4F2F7&border-radius=8%2C8%2C8%2C8&border-radius-inner=8%2C8%2C8%2C8&blend-align=bottom&blend-mode=normal&blend-x=0&blend-w=1200&blend64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmstdjIucG5n&mark-x=2&mark-y=3&m64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL2JsYW5rLnBuZz9tYXNrPWNvcm5lcnMmYm9yZGVyPTQlMkNGRjc0NDImdz0xMTk3Jmg9MzYmZml0PWNyb3AmY29ybmVyLXJhZGl1cz0xMA%3D%3D)

<br/>

***


**Commands Used:**
```bash
# Most important commands from today
cls - to list directiories
pwd - print working directiories
whoami - show information about the user
```

**Result:** [What works now]

**Screenshots:** [Yes/No - saved in ./screenshots/]

Key pair permission before changing to allow SSH (./screenshots/apache-web-server-key-pair-permission-setting-before.png)

Changed permission to the key pair(./screenshots/key-pair-permission-setting-changed.png)

SSH into the EC2 Instance(./screenshots/ssh-to-ec2-instance.png)

Install Apache Web Server(./screenshots/updating-instance-and-installing-apache-web-server.png)



---

## 💡 Key Learning

**One thing I'll remember from today:**
[The most important concept or skill]

**How I'll use it:**
[Practical application]

---

## 🐛 Problems Faced

**Problem:** [Brief description]  
**Solution:** [How you fixed it]  
**Lesson:** [What you learned]

---

## 💰 AWS Resources

**Created Today:**
- [Resource 1] - [Status: Running/Stopped]
- [Resource 2] - [Status: Active/Deleted]

**Cleanup Status:**
- [ ] All resources stopped/terminated
- [ ] Billing checked: $[X.XX]

---

## 📅 Tomorrow

**Focus:** [Tomorrow's topic]

**To-Do:**
- [ ] Task 1
- [ ] Task 2
- [ ] Task 3

**Questions to Answer:**
- [Question 1]
- [Question 2]

---

## ✅ Quick Check

- [ ] Learned something new
- [ ] Built something working
- [ ] Documented progress
- [ ] Cleaned up AWS resources
- [ ] Updated main README
- [ ] Committed to GitHub

---

**Daily Win:** [One thing you're proud of today]

**Tomorrow's Promise:** [One commitment for tomorrow]

---

**Day 3/90 Complete** ✓