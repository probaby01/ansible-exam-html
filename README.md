# Static HTML for Nginx Deployment

This repository contains the **HTML file used for automated deployment via Ansible** to two AWS EC2 instances running Nginx. The project was part of my **AltSchool Africa Cloud Engineering 2nd Semester Examination**, where I deployed a website using:

- **AWS EC2 + Classic Load Balancer**
- **Ansible Automation**
- **AWS S3 Static Website Hosting**

---

## 🔗 Project Links

| Resource | Link |
|----------|------|
| **Medium Article (Full Documentation & Story)** | https://medium.com/@asomad4islam/from-ec2-to-s3-automating-website-deployment-with-ansible-on-aws-altschool-project-8be8b71db257 |
| **GitHub Repo (Current)** | https://github.com/probaby01/ansible-exam-html |
| **S3 Static Website URL** |  https://us-east-1.console.aws.amazon.com/s3/object/exam-static-site-muhammed?region=us-east-1&bucketType=general&prefix=index.html|
| **Load Balancer DNS URL** | http://exam-classic-lb-1578794954.us-east-1.elb.amazonaws.com |

---

## 🛠️ How This HTML Is Used

This file is deployed automatically via Ansible using:

```yaml
- name: Deploy index.html using template
  template:
    src: index.html.j2
    dest: /var/www/html/index.html

---

## 📌 Credits

This project was completed as part of the **AltSchool Africa Cloud Engineering Program**.

**Author:** *Muhammed Abdulsamad*
