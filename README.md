# IAAC-Project-CloudFormation
**CloudFormation Template: Infrastructure Deployment**

This project was made by:
Lior Matana




This repository contains a CloudFormation template for deploying the following infrastructure resources on AWS:

- Virtual Private Cloud (VPC)

- Subnets (Public and Private)

- Internet Gateway

- NAT Gateway

- Route Tables

- Security Groups

- EC2 Instances (Bastion, WebServer, AppServer)

- RDS Database Instance

  
The architecture is taken from AWS re/Start Grad Training - V2- Project 1 Lab:  Highly Available 3-Tier Architecture.

After completing the Lab through the Console, I challenged myself to do the same architecture by IAAC- CloudFormation.



**Architecture**


![Tier3Topology (2)](https://github.com/liormat401/IAAC-Project-CloudFormation/assets/126070709/b6e9276e-6f7a-4194-83dd-6da06a3cd967)
*Architecture from AWS Training Lab*

![template1-designer (2)](https://github.com/liormat401/IAAC-Project-CloudFormation/assets/126070709/282dd833-f10d-4cb6-a15b-165f086fd18e)
*Automated architecture made by CloudFormation Designer, according to my stack/template.*


**Deployment**

*Pay Attention: It is a SEVERE SECURITY VULNERABILITY to use the tamplete as is. you MUST change the DB user and password.*
1. Open Console on CloudFormation
2. Create Stach >> With New resources(standard)
3. Template source: Upload a template file
4. Template Name for your choosing
5. Tags-Optional but recommended

   
OR by CLI:
aws cloudformation create-stack stack-name myteststack template-body file://file.json

Enjoy the green:)
![image](https://github.com/liormat401/IAAC-Project-CloudFormation/assets/126070709/81cb18d4-dad5-4326-a36f-27ab93187153)


  
     
**Special Thanks**

This project was tough for me as I never used CloudFormation or wrote anything in JSON format.
Here are resources that helped me a lot starting and troubleshooting along the way.

- https://start.jcolemorrison.com/the-complete-cloudformation-guide-setting-up-our-series-project/
- https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html
- https://stackoverflow.com/questions/66131377/how-to-attach-elastic-ip-to-natgateway-via-cloud-formation
- AWS Project 1 Lab Guide- Although it's a guide for the Console, it did help me configure one resource at a time. (is added as "Tier 3 Master Level Instructions")
  
And how not, ChatGPT for always finding my missing commas of brackets.















