# CMPE282-Homework-1-Active-Directory

Create an AWS Directory Service AD in AWS and Populated with users from the sample user database having large dataset of (300K+ users).

## Configure the AWS Managed Active Directory Domain Services (DS AD):
- Input Directory DNS Name.
- Provide Admin Password for Active Directory.
- Select the VPC and host subnets in different availability zones.

![image](https://user-images.githubusercontent.com/40047632/219298610-4fd7f9fc-9dee-4e6b-b201-d3c3f5295cf4.png)

## Launch EC2 instance and Select Microsoft OS image:
- Connect to Microsoft EC2 Instance.
- Set DNS address of Directory Service created in AWS, inside Internet Protocol(TCP/IPv4) Properties.
- Set the Domain name of Directory Service, inside Advance System Setting > Computer Name 
- Now we are connected to our created Active Directory i.e “corp.fourmusks.com”

![image](https://user-images.githubusercontent.com/40047632/219298744-35e96457-0ea9-464d-99bf-639fa6b31f03.png)

![image](https://user-images.githubusercontent.com/40047632/219299990-a27289e0-b9d5-4a2e-8d7b-6fd852e6d6cf.png)

## Import Users in AD from large dataset of (300K+ users):
- Download data from large dataset (300K+ users) <br />
https://raw.githubusercontent.com/datacharmer/test_db/master/load_employees.dump
- Convert the data related to the attribute fields that need to be inserted into Active Directory into a CSV file. 
- Then use a PowerShell script to add the user data one at a time to Active Directory

![image](https://user-images.githubusercontent.com/40047632/219300616-940199c4-c224-4c79-8ae6-f63d6641cb9f.png)

![image](https://user-images.githubusercontent.com/40047632/219300669-7c20d6e8-601a-4e79-a656-a75250eab929.png)

**Total Count of Users imported: 78857**

![image](https://user-images.githubusercontent.com/40047632/219300720-67f7bea6-e0d1-41a8-b876-2de063e7c3a6.png)
