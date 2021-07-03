##############################################
01-SimpleWebserver is Infrastrcture as code Cloudformation script for an apache webserver deployed in a AWS Virtual Private Container.
There is a YAML file and a JSON parameters file. 
The parameters file for this and subsequent Cloudformation scripts is to ensure parameter values are decoupled from the main script for easier maintenace
##############################################
02-cloudNetwork is another Cloudformation script for a cloud network that includes
-A VPC
-Public and Private Subnets
-An Internet Gateway
-A NAT Gateway
-Routing Tables

The cloud network was created with with high availability in mind. Hence we can see the subnets are split in two availability zones.
Elastic IPs were used in order to ensure that the same IP is associated with the Internet gateway. 
The cloud diagram 02-CloudNetwork.jpeg was created in Lucidchart and is partially implemented in the cloudformation script 
###############################################
