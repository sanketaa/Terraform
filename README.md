# Terraform Multi-Cloud Infrastructure Labs

A collection of hands-on infrastructure-as-code labs covering Terraform fundamentals and progressively more complex deployment scenarios across AWS, Google Cloud, and Microsoft Azure.

## Background

This repository documents practical Terraform exercises completed to build experience with reusable infrastructure, cloud networking, compute, data services, containers, configuration management, image creation, and multi-cloud deployment patterns.

The folders are organized by learning section and job-style case study. They are educational labs, not a single production platform. Each example should be reviewed and updated before use because provider versions, machine images, modules, and cloud-service interfaces can change.

## Topics Covered

- Terraform installation, syntax, state, variables, outputs, and resource dependencies
- Reusable modules for EC2 and load-balancing infrastructure
- AWS web application infrastructure
- Amazon DynamoDB
- Kubernetes deployment with kOps and Docker
- Amazon EKS
- Elastic Load Balancing and EC2
- ELK stack infrastructure
- Amazon Aurora
- Terraform with Ansible
- Packer image-building examples
- Google Cloud managed instance groups
- Microsoft Azure infrastructure

## Repository Map

| Directory | Focus |
| --- | --- |
| `Section2_Firststepswithtf` | Terraform fundamentals |
| `Section3_Usingvariables` | Variables and configurable infrastructure |
| `Section7_Jobcasestudy#1_Webapp` | AWS web application case study |
| `Section8_Jobcasestudy#2_Dynamodb` | DynamoDB case study |
| `Section9_Jobcasestudy#3_KOPSandDocker` | Kubernetes, kOps, and Docker |
| `Section10_Jobcasestudy#4_EKScluster` | Amazon EKS cluster |
| `Section11_Jobcasestudy5_ModulesELBEC2` | Terraform modules, ELB, and EC2 |
| `Section13_Jobcasestudy6_ELK` | ELK infrastructure |
| `Section16_Jobcasestudy#7_Auroracluster` | Amazon Aurora cluster |
| `Section19_Jobcasestudy8_TerraformGCP` | Google Cloud autoscaling infrastructure |
| `Section20_Jobcasestudy9_TerraformAzure` | Microsoft Azure infrastructure |
| `AnsibleandTerraform` | Terraform and Ansible integration |
| `Packerexamples` | Machine-image creation with Packer |

## Technologies

- Terraform and HashiCorp Configuration Language (HCL)
- Amazon Web Services
- Google Cloud Platform
- Microsoft Azure
- Kubernetes, Amazon EKS, and kOps
- Docker
- Ansible
- Packer
- ELK stack

## Skills Demonstrated

- Translating infrastructure requirements into declarative code
- Parameterizing deployments with variables and outputs
- Organizing reusable infrastructure with modules
- Provisioning compute, networking, load-balancing, database, and container resources
- Combining provisioning with configuration-management and image-building tools
- Comparing infrastructure patterns across multiple cloud providers

## Safe Usage

These labs can create billable cloud resources. Review the code in the selected directory before running it.

Typical workflow:

```bash
terraform fmt
terraform init
terraform validate
terraform plan
terraform apply
```

When the lab is complete:

```bash
terraform destroy
```

Use current provider documentation, verify regions and resource names, and apply least-privilege permissions. Never commit credentials, private keys, Terraform state files, or secrets.

## Portfolio Context

This repository shows the progression from basic Terraform concepts to broader infrastructure case studies. The most relevant examples for cloud and DevOps work are the EKS, EC2/ELB modules, Aurora, ELK, Ansible/Terraform, Packer, GCP, and Azure sections.
