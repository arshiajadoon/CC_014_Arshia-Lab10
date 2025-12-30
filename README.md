Lab 10 – GH CLI Codespaces + AWS + Terraform: CLI Automation of VPC/Subnet Creation


Student Name: Arshia Jadoon
Roll Number: BSE-2023-014
Course: Cloud Computing
Instructor: Sir Waqas Saleem
Institution: Fatima Jinnah Women University (FJWU)

📌 Lab Overview
This lab focuses on Infrastructure as Code (IaC) using Terraform and AWS CLI. The objective is to set up a cloud development environment using GitHub Codespaces, configure AWS CLI, write Terraform configurations to provision a VPC and subnet, manage Terraform state, and understand Terraform operations like plan, apply, destroy, and output.

✅ Tasks Performed
Task 1: Setting Up GitHub Codespaces
Authenticated with GitHub.

Created and connected to a GitHub Codespace via SSH.

Used the terminal within Codespaces to execute cloud and Terraform commands.

Task 2: Installing and Configuring AWS CLI & Terraform
Installed AWS CLI and verified the version.

Configured AWS CLI with credentials (aws configure).

Verified identity using aws sts get-caller-identity.

Installed Terraform and checked its version.

Created a main.tf file with the AWS provider block.

Initialized Terraform with terraform init.

Task 3: Provisioning AWS VPC & Subnet Using Terraform
Added AWS VPC and subnet resources in main.tf.

Applied the configuration using terraform apply.

Verified the created VPC and subnet using AWS CLI.

Task 4: Terraform State & Lifecycle Management
Used terraform plan to preview changes.

Applied changes with terraform apply.

Targeted destruction of specific resources with terraform destroy -target.

Applied terraform refresh and reapplied configurations.

Added and removed tags to understand update behavior.

Destroyed all resources with terraform destroy.

Task 5: Terraform State File Management
Checked the Terraform state file after destruction.

Created a backup of the previous state.

Reapplied Terraform to repopulate the state file.

Listed resources in the state with terraform state list.

Showed details of a resource using terraform state show.

Task 6: Terraform Outputs
Defined and used output blocks to display resource attributes.

Retrieved values such as VPC ID and subnet ID.

Cleanup
Destroyed all resources at the end of the lab using terraform destroy.

📁 Files & Artifacts
File Name	Description
main.tf	Contains AWS provider, VPC, subnet, and output configurations
terraform.tfstate	Terraform state file (managed automatically)
task1_codespace_ssh_connected.png	Screenshot of SSH connection to Codespace
task2_aws_configure_and_files.png	AWS CLI configuration proof
task3_terraform_apply_vpc_subnet.png	Terraform apply execution
task4_terraform_destroy_targeted.png	Targeted resource destruction
task5_terraform_state_list.png	Terraform state list output
task6_terraform_outputs_basic.png	Terraform outputs example
🧠 Key Learnings
Hands-on experience with GitHub Codespaces as a cloud-based IDE.

Configuration and use of AWS CLI for cloud operations.

Writing Terraform configurations to define cloud infrastructure.

Understanding Terraform workflow: init, plan, apply, destroy.

Managing Terraform state and performing state operations.

Using Terraform outputs to extract resource information.

Practicing IaC best practices for reproducible and version-controlled infrastructure.

🛠️ Tools & Technologies Used
GitHub Codespaces

AWS CLI

Terraform

AWS (VPC, Subnet)

Bash Terminal

🧹 Cleanup Instructions
At the end of the lab, ensure all AWS resources are destroyed to avoid unnecessary charges:

bash
terraform destroy -auto-approve
🏁 Conclusion
This lab provided a comprehensive introduction to Infrastructure as Code using Terraform on AWS. It covered environment setup, resource provisioning, state management, and clean destruction, reinforcing the principles of repeatable, automated, and version-controlled infrastructure deployment in the cloud.

Submitted by: Arshia Jadoon
Roll Number: BSE-2023-014
