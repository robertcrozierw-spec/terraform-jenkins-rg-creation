# terraform-jenkins-rg-creation
The objective of this repo is to create a resource group in Azure via Terraform script and Jenkins pipeline.

Authentication between Jenkins and Azure will be done via service principal.

The statefile will initially be stored on the Jenkins server, however later I will be storing it in a storage account to be referenced by other Terraform projects.