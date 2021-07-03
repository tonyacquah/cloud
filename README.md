

01-SimpleWebserver is Infrastrcture as code utilizing AWS Cloudformation for an apache webserver deployed in a AWS Virtual Private Container.
There is a YAML file and a JSON parameters file. 
The parameters file is used to ensure resource instance values are not hardcoded in the YAML Cloudformation Template file. This allows for easier maintenace

02-cloudNetwork is another Cloudformation file for a cloud network that includes
-A VPC
-Public and Private Subnets
-An Internet Gateway
-A NAT Gateway
-Routing Tables

The cloud network was created with with high availability in mind. Hence we can see the subnets are split in two availability zones.
Elastic IPs were used in order to ensure that the same public IP is consistently associated with the Internet gateway after first assignment. 
The cloud diagram 02-CloudNetwork.jpeg was created in Lucidchart and is partially implemented in the cloudformation script 
