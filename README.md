# WordpressWebsite
Deployed and hosted a highly-available WordPress website called cloudnotesforfree on AWS using EC2, RDS, Route 53, ASG, and VPC.

Reference Architecture: 
![1_WordPress_Project_Reference_Architecture](https://github.com/sgummal2/WordpressWebsite/assets/140002588/80924ba1-2fe5-4c84-932e-b02ae5070246)

#**Here's a breakdown of the key components and concepts involved:**

•	**VPC with Public and Private Subnets**: Creating a Virtual Private Cloud (VPC) with public and private subnets in multiple availability zones ensures network isolation and availability.

•	**Internet Gateway**: Facilitates communication between instances within the VPC and the internet.

•	**Availability Zones**: Using multiple availability zones enhances high availability and fault tolerance by distributing resources across 
   different physical data centers.

•	**Nat Gateway and Bastion Host**: These resources provide secure access to instances in private subnets and allow outbound internet connectivity for those instances.

•	**Resources Placement**: Placing web servers and database servers in private subnets enhances security by limiting direct exposure to the internet.

•	**MySQL RDS Database**: Amazon RDS provides a managed relational database service that supports the WordPress application.

•	**Amazon EFS**: Using Amazon Elastic File System (EFS) allows shared file storage for web servers.

•	**EFS Mount Targets**: EFS mount targets in each AZ provide access to the shared file storage.

•	**EC2 Instances**: Hosting the website on EC2 instances allows you to customize the environment to suit your needs.

•	**Application Load Balancer**: Distributes incoming web traffic across an Auto Scaling Group of EC2 instances for load balancing and fault 
   tolerance.

•	**Auto Scaling Group**: Creates and manages a dynamic group of EC2 instances to automatically adjust capacity based on demand.

•	**Route 53**: Amazon Route 53 is used to register the domain name and create DNS records for routing traffic to the website.


**Steps used to deploy WordPress website On AWS:**

•	Created an Application Load Balancer

•	Built a Three-Tier AWS Network VPC from Scratch

•	Created Nat Gateways

•	Created the Security Groups

•	Created the RDS Instance

•	Created the Elastic File System (EFS)

•	Installed WordPress

•	Created an Application Load Balancer

•	Registered a New Domain Name in Route 53

•	Created a Record Set in Route 53

•	Registered for an SSL Certificate in AWS Certificate Manager

•	SSH into Instance in the Private Subnet

•	Created an HTTPS Listener for the Application Load Balancer

•	Created an Auto Scaling Group

•	Installed WordPress Theme and Template


Images:
<img width="960" alt="1" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/2c30a6a8-0406-4b67-87b6-c9e1056bbec9">
<img width="960" alt="2" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/d932289c-2a6d-4277-ab55-904fc6d4b691">
<img width="960" alt="3" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/4a8f36fb-be5d-4520-a024-1e4fb17cdaa6">
<img width="960" alt="4" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/26ba1b9b-c642-4084-855e-ab35a84cf89e">
<img width="960" alt="5" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/a3ee8185-0884-4745-b797-a00f2e86d32b">
<img width="960" alt="6" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/92bc0dc5-9ffc-45c1-bd35-b93d0cf6a230">
<img width="960" alt="7" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/160e640e-8456-45d2-b265-5e8aebc6ce59">
<img width="960" alt="8" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/5d122ed1-6596-4c14-b8f1-833d8f0f4112">
<img width="960" alt="9" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/cd3d27e4-3e75-4b04-aa11-c505cfd32e27">
<img width="960" alt="10" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/2ced1503-2a3d-48d4-befe-392f3bb5e44b">
<img width="960" alt="11" src="https://github.com/sgummal2/WordpressWebsite/assets/140002588/8a08de04-9d72-4e2b-b654-9d790cbe825c">













