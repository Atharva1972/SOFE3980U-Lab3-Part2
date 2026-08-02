\# SOFE3980U Lab 3 Part 2 - CI/CD using Jenkins on GKE



\*\*Atharva Rajadhyaksha - 101041016\*\*



\## Contents

\- `BinaryCalculatorWebapp/` - Maven Spring Boot Binary Calculator app (Add, OR, AND, Multiply), with Dockerfile, Jenkinsfile (script-based CI job), and Jenkinsfile\_v2 (full CI/CD pipeline)

\- `jenkins/values.yaml` - Helm configuration used to install Jenkins on the GKE cluster



\## Jenkins Jobs

\- `binaryCalculate\_mvn` - Maven project job (UI-configured CI)

\- `BinaryCalculator\_pipeline` - Jenkinsfile-based pipeline job (script-based CI)

\- `BinaryCalculator\_cicd` - full CI/CD pipeline using Jenkinsfile\_v2 (test, build, containerize, deploy, expose)



\## Summary

\- Jenkins installed on the existing `sofe3980u` GKE cluster via Helm

\- CI configured two ways: a UI-configured Maven job and a Jenkinsfile-based pipeline job

\- Full CI/CD pipeline set up using a GCP service account, Kubernetes cloud connection in Jenkins, and Jenkinsfile\_v2 - automatically tests, builds, containerizes, pushes to Artifact Registry, and deploys to GKE on every commit

\- Design task: added OR, AND, and Multiply operations to the Binary Calculator, verified the CI/CD pipeline automatically redeployed the updated application

Test 1
Test 1.1 
Test 1.2
Test 1.3
Test 1.4