# Terraform snippet for deploying ASG in private subnet behind ALB

 Below is the architecture to be implemented:
 ![arch](https://user-images.githubusercontent.com/70053804/118510517-a8aa5780-b74e-11eb-881c-351648f3335c.png)

The files included are:

    a)  main.tf: main.tf file contains the terraform script to create necessary resources.
    b)  variables.tf: for declaring variables being used in the main script
    c)  terraform.tfvars: for defining/overriding the varibles
    d)  init_webserver.sh: User data script for launch config which installs & starts nginx server and creates mount points
       
# Prerequisites:
 
 1.  AWS account 
 2.  IAM role with necessary permissions
 3.  Terraform & AWS CLI configured on machine from which the scripts are to be run
