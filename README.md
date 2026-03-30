# CI/CD Basics

## 01) What is CI/CD?

**CI/CD** stands for **Continuous Integration** and **Continuous Deployment/Delivery**.

- **Continuous Integration (CI):**
  Developers frequently merge their code into a shared repository. Each change is automatically tested and built to detect issues early.

- **Continuous Delivery (CD):**
  Code changes are automatically prepared for release to production.

- **Continuous Deployment (CD):**
  Every change that passes testing is automatically deployed to production without manual approval.

---

## 02) Three Tools of CI/CD

Here are some popular CI/CD tools:

- Jenkins  
- GitHub Actions  
- GitLab CI/CD  

---

## 03) What is Jenkins Pipeline?

A **Jenkins Pipeline** is a suite of plugins that allows you to define your build, test, and deployment process as code.

- It is written in a file called `Jenkinsfile`
- It automates the CI/CD workflow
- It defines stages like build, test, and deploy

---

## 04) What language is Jenkins based on?

Jenkins is based on **Java**.

---

## 05) What scripting language is Jenkins Pipeline syntax based on?

Jenkins Pipeline syntax is based on **Groovy**.

---

## 06) Ways to Write Pipeline in Jenkins

There are two main ways:

1. **Declarative Pipeline**
   - More structured and simple
   - Easier to read and maintain
   - Example:
     ```groovy
     pipeline {
         agent any
         stages {
             stage('Build') {
                 steps {
                     echo 'Building...'
                 }
             }
         }
     }
     ```

2. **Scripted Pipeline**
   - More flexible
   - Written entirely in Groovy
   - Example:
     ```groovy
     node {
         stage('Build') {
             echo 'Building...'
         }
     }
     ```

---

## Author

Mostafa Mohamed