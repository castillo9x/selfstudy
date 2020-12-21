# Infrastructure As Code with Terraform and Ansible
## Terraform

### What is Terraform?
Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.


![Terraform keys](assets/Terraform1.png)

## CloudFormation
### What is AWS CloudFormation?
AWS CloudFormation is a service that gives developers and businesses an easy way to create a collection of related AWS and third-party resources, and provision and manage them in an orderly and predictable fashion.

![ClouFormation keys](assets/cf-definition.png)

## Ansible
### What is Ansible?
Ansible is a radically simple IT automation engine that automates cloud provisioning, configuration management, application deployment, intra-service orchestration, and many other IT needs.


![Terraform keys](assets/ans-definition.png)

## Comparative chart
![Terraform keys](assets/iac-compare.png)

## Install Terraform
Add the HashiCorp GPG key.

`curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -`

Add the official HashiCorp Linux repository.

`sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"`

Update and install.

`sudo apt-get update && sudo apt-get install terraform`

