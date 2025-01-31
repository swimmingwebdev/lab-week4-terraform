# lab-week4-terraform

### Instructions to configure the infrastructure using Terraform

- step 1. Create new SSH keypair using `ssh-keygen`
- step 2. Add public key to cloud-init config file `cloud-config.yaml`
- step 3. Add packages to install `nignx` and `nmap` in `cloud-config.yaml`
- step 4. configure terrafrom `main.tf`

- step 5.  rewrite Terraform config file to canonical format `terraform fmt`
- step 6. check for syntax errors `terraform validate`
- step 7. initialize terraform `terraform init`
- step 8. creates an execution plan `terraform plan -out <plan-name>`
   - If you have an error ` Error: No valid credential sources found`, \
   ensure that you have installed the **AWS CLI** 
   - If **AWS CLI** is not installed,
      1. Install using `sudo apt update && sudo apt install awscli -y`
      2. Set up AWS Credentials using `aws configure`
- step 9.  executes actions in Terraform plan `terraform apply`
- step 10. destroy all remote objects `terraform destroy`
