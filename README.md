# Terraform snippet for deploying ASG in private subnet behind ALB

 Below is the architecture to be implemented:

![image](https://user-images.githubusercontent.com/70053804/119807062-662c0c00-bf00-11eb-97f9-1a463a48ec0b.png)


The files included are:

    a)  main.tf: main.tf file contains the terraform script to create necessary resources.
    b)  variables.tf: for declaring variables being used in the main script
    c)  terraform.tfvars: for defining/overriding the varibles
    d)  init_webserver.sh: User data script for launch config which installs & starts nginx server and creates mount points
       
# Prerequisites:
 
 1.  AWS account 
 2.  IAM role with necessary permissions
 3.  Terraform & AWS CLI configured on machine from which the scripts are to be run
