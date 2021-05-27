# Terraform snippet for deploying ASG in private subnet behind ALB

 Below is the architecture to be implemented:
 ![arch]![image](https://user-images.githubusercontent.com/70053804/119806683-0df50a00-bf00-11eb-9155-bcfbbb5cc891.png)


The files included are:

    a)  main.tf: main.tf file contains the terraform script to create necessary resources.
    b)  variables.tf: for declaring variables being used in the main script
    c)  terraform.tfvars: for defining/overriding the varibles
    d)  init_webserver.sh: User data script for launch config which installs & starts nginx server and creates mount points
       
# Prerequisites:
 
 1.  AWS account 
 2.  IAM role with necessary permissions
 3.  Terraform & AWS CLI configured on machine from which the scripts are to be run
