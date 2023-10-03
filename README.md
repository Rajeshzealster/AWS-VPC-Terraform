# AWS-VPC-Terraform
Creation of VPC and deploy 2 applications in different availability zones while also creating a load balancer to balance the load between the instances automatically.
# AWS VPC Deployment with Terraform

This project demonstrates the deployment of an Amazon Virtual Private Cloud (VPC) using Terraform. The VPC is designed to host two applications in different availability zones, ensuring high availability and fault tolerance. Additionally, we will create an Elastic Load Balancer (ELB) to automatically balance the load between the instances.

## Prerequisites

Before you begin, ensure you have the following prerequisites in place:

1. **AWS Account**: You must have an AWS account with the necessary IAM permissions.

2. **Terraform**: Install Terraform on your local machine. You can download it from the [Terraform website](https://www.terraform.io/downloads.html).

3. **AWS CLI**: Install and configure the AWS CLI on your local machine.

## Deployment Steps

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/aws-vpc-terraform.git
cd aws-vpc-terraform
```
### Step 2: Configure AWS Credentials
Ensure your AWS credentials are configured. You can do this by running aws configure and providing your AWS Access Key ID and Secret Access Key.

### Step 3: Initialize Terraform
```bash
terraform init
```
This command initializes the Terraform working directory and downloads the required providers.

### Step 4: Create and Deploy the VPC
```bash
terraform apply
```
Review the execution plan, and when prompted, type yes to create the VPC and associated resources.
### Step 5: Access the Applications
After the deployment is complete, Terraform will output the URLs for accessing your applications and the load balancer.

### Step 6: Cleaning Up
To destroy the resources created by Terraform when you're finished, run:
```bash
terraform destroy
```

Review the execution plan and type yes when prompted.

## Project Structure
The project structure includes the following key files:

**main.tf**: Defines the AWS resources, including VPC, subnets, instances, and the Elastic Load Balancer.

**variables.tf**: Declares input variables used in the configuration.

**outputs.tf**: Specifies the outputs that Terraform will display after deployment.

**terraform.tfvars:** Stores your AWS access key, secret key, and any other sensitive information. Be sure to keep this file secure and not commit it to version control.

## Conclusion
This project demonstrates how to deploy an AWS VPC with Terraform, hosting two applications in different availability zones and automatically balancing the load between them using an Elastic Load Balancer. You can customize the configuration to suit your specific requirements.

For questions or assistance, feel free to reach out to the project maintainers:

Rajesh thalla - <rajeshzealster@gmail.com>
Happy coding!



