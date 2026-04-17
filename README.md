# Jenkins Freestyle CI/CD with Master–Slave Architecture (JAR & WAR Deployment)

## 📌 Description

This project demonstrates a CI/CD setup using Jenkins Freestyle Jobs with Master–Slave architecture. The Jenkins master manages job execution, while slave nodes handle JAR and WAR builds. WAR artifacts are deployed to Apache Tomcat, and artifacts are stored in Nexus. Git webhooks enable automated builds on code commits.

---

## 🔗 Reference Repositories

* JAR Project Repo: https://github.com/navyasrigondela45/Java-Web-Application-JAR-Build-Deployment-using-Maven-on-EC2.git
* WAR Project Repo: https://github.com/navyasrigondela45/Java-WAR-Deployment-with-Jenkins-Tomcat-Nexus-CI-CD-.git

👉 These repositories can be used to replicate the setup on slave nodes.

---

## 🏗️ Architecture

Developer → Git Push → Webhook → Jenkins Master → Slave Nodes → Build → Nexus → Deploy (Tomcat)

---

## ⚙️ Jobs Overview

* **JAR Job** → Builds JAR using Maven on Slave Node 1 and stores artifact in Nexus
* **WAR Job** → Builds WAR on Slave Node 2, stores artifact in Nexus, and deploys to Apache Tomcat

---

## 🛠️ Tools Used

* Jenkins (Freestyle Jobs)
* GitHub
* Maven
* Apache Tomcat
* Nexus Repository Manager
* Linux (EC2 Instances as Slave Nodes)

---

## 📊 Outputs

* EC2 instances view:
* 
<img width="1537" height="475" alt="image" src="https://github.com/user-attachments/assets/53a4e46e-642e-4dc7-852c-8a9fdb1d5536" />

* Webhook-trigger on both the repos:
  
  <img width="1918" height="947" alt="image" src="https://github.com/user-attachments/assets/86ddc5cc-8b9e-40f6-95b8-c719c79ef3cb" />
  <img width="1918" height="947" alt="image" src="https://github.com/user-attachments/assets/bb4ee022-4323-4bcf-879a-b651e79feb22" />

* Jenkins Dashboard:
  
  <img width="1918" height="626" alt="image" src="https://github.com/user-attachments/assets/54580ddd-fee2-49f1-b148-0ed358e6a18f" />
  
* Successful JAR build (console output)
  <img width="1918" height="780" alt="image" src="https://github.com/user-attachments/assets/82e6b4f6-778a-4bb5-b5c4-b48f8d856337" />

* Successful WAR build and deployment
  <img width="1918" height="578" alt="image" src="https://github.com/user-attachments/assets/0dd247ca-fc81-482d-b15c-dd9618fc7cd3" />
  <img width="1920" height="610" alt="image" src="https://github.com/user-attachments/assets/64591882-3211-454a-90d3-9f69a75062d6" />

* Artifact stored in Nexus repository
  <img width="1245" height="607" alt="image" src="https://github.com/user-attachments/assets/9a57390e-15bd-4d37-b914-263c1d1b317d" />
  <img width="1242" height="543" alt="image" src="https://github.com/user-attachments/assets/aff84d66-f275-4229-875c-f8aae014a797" />

* Application running (JAR) on browser:
  <img width="1918" height="652" alt="image" src="https://github.com/user-attachments/assets/3b3dcf9c-a24c-40b1-a823-5b1d23a97953" />

* Application running on Tomcat (browser output)
  <img width="1918" height="641" alt="image" src="https://github.com/user-attachments/assets/e4dbcab9-214c-4a59-a797-e3adf7c7ef02" />

* Jenkins slave nodes
  <img width="1918" height="660" alt="image" src="https://github.com/user-attachments/assets/28b7a6c6-5e04-49e7-a6a8-5536c85882bd" />

---

## 🚀 Future Improvements

* Convert Freestyle Jobs to Jenkins Pipeline (Jenkinsfile)

