# terraform-jenkins-rg-creation
The objective of this repo is to create a resource group in Azure via Terraform script and Jenkins pipeline.

Authentication between Jenkins and Azure will be done via service principal.

The statefile will initially be stored on the Jenkins server, however in later projects I will be storing it in a storage account to be referenced by other Terraform projects.

## Prerequisites 
An azure subscription.
A service principal with appropriate RBAC permissions to said above subscription.
A credential configured in Jenkins with the above Service Principal.

## Included Files
The two files included are:
-   main.tf - this is the terraform file used to describe the resources and provider needed.
-   Jenkinsfile - The actual pipeline code to run.


