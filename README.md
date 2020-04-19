## Udacity Nanodegree Program - Cloud Devops Track


### Project 1 - Deploy Static Website on AWS
In this project, a static website was deployed to AWS using S3, CloudFront, and IAM.
Below is a link to te website:
http://d1as6hos5gbo9k.cloudfront.net/index.html


### Project 2 - Deploy a high-availability web app(Udagram) using CloudFormation
In this project, a high-availability web app was deployed using CloudFormation. 

#### Problem
Your company is creating an Instagram clone called Udagram. Developers pushed the latest version of their code in a zip file located in a public S3 Bucket.

You have been tasked with deploying the application, along with the necessary supporting software into its matching infrastructure.

This needs to be done in an automated fashion so that the infrastructure can be discarded as soon as the testing team finishes their tests and gathers their results.

#### Cloud Architecture for Udagram

Below is the Cloud architect diagram for the stack created
![Cloud Architecture Diagram](https://github.com/ivan-claire/Udacity-Cloud-Devops-Nanodegree/CloudArchitectDiagram.png.png)


A Launch Configuration for the application servers was created in order to deploy four servers
and a bastion host was setup inorder to SSH into the private subnet servers.

#### Stack Creation order
##### Network Stack
HA-network.yml and network-params.json
##### BastionHost Stack
HA-bastion-server.yml and bastion-server-params.json
##### ServerInfrastructure
HA-server.yml and server-params.json

#### Run the Program
use the create_stack.sh and update_stack.sh files to create the stacks.

