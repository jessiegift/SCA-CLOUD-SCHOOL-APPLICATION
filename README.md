# SCA-CLOUD-SCHOOL-APPLICATION
Below were steps taken to achieve Task num 1:

## step 1 - Preparation of my environment.
For this task, I created an Azure account. To create an azure account visit  portal.azure.com.

Created a Linux virtual machine to host my Jenkins.

Added an inbound port rule 8080 and also made my IP address static (20.86.110.254)

Created a Docker account for deployment which will be discussed later.

## step 2 -  Jenkins Setup

A prerequisite for installing Jenkins is the installation of Java.

After connecting to the Linux VM. I installed Java

Install Jenkins on the Virtual machine, started the development server, and created an administrative user.

Installed Suggested Plugins

Username: jessiegifted  
Password:08035656928


## step 3 - Create a build Job
Created a build Job named SCA cloud 1
![IMG-20210722-WA0010](https://user-images.githubusercontent.com/87488892/126787109-71e831bf-0377-4a8a-a760-8ca1dd7a3596.jpg)

Used a Declarative Pipeline syntax by creating a Jenkins file in my Github repo.

Installed a nodejs plugin in my Jenkins server as my app is running using NodeJS, also, the tool used in the Jenkins fine is a nodejs tool.

Added my Github Credentials and integrated my repro successfully to Jenkins as seen below.
![build and deploy successful](https://user-images.githubusercontent.com/87488892/126696742-f15debfc-acfa-460d-b422-1f931eec0919.PNG)

## step 4 - Deployment
Create a repository in the Docker account created from step 1

Created a Docker file in my Github

Installed a Docker Plugin in my Jenkins server

Installed Docker also in my Linux VM

Then Build again as seen in the below screenshot.
![deploy sucess original](https://user-images.githubusercontent.com/87488892/126696793-0ceb8ca8-60f3-49e7-ad20-f95f39462086.PNG)


## Notes
Username jessiegifted

Password 08035656928

Jenkins Url 20.86.110.254:8080

If the server isn't available, that means my azure credit finished before the assessment. Do not hesitate to contact me at onyinyeonomesky@gmail.com

## Ref

https://www.digitalocean.com/community/tutorials/how-to-install-jenkins-on-ubuntu-20-04

https://www.jenkins.io/doc/book/pipeline/syntax/

https://docs.cloudbees.com/docs/admin-resources/latest/pipeline-syntax-reference-guide/declarative-pipeline

https://docs.docker.com/engine/install/ubuntu/

