---
<h1>AKS Cluster application deployment with ACR, CICD using Jenkins</h1>

 

<h2>Description</h2>
In this project, i embarked on a strategy to streamline manual deployments to AKS via ACR
and implement an automated CI/CD pipeline using Jenkins. The goal is to enhance the efficiency,
reliability, and scalability of my application deployment process. 
I started with manual deployment of Azure Kubernetes Service (AKS) and Azure Container Registry
(ACR). These are critical preparatory steps before diving into automation CI/CD with
Jenkins. 
During manual deployments, i was able to thoroughly test and validate the application in the AKS
environment. This involved making sure that all components worked seamlessly within the
Kubernetes cluster and fine-tuned configurations for optimal performance. 
Additionally, the manual deployment allowed for in-depth technical scrutiny. 
Integration testing, another critical aspect, was carried out during manual deployments to
confirm that all parts of my application worked together harmoniously within AKS. 
<br />


<h2>Tools</h2>

- <b>Github</b> 
- <b>Azure Kubernetes Service (AKS)</b>
- <b>Azure Container Registry (ACR)</b>    
- <b>Jenkins</b>
- <b>Azure Kubernetes Cluster</b>

<h2>Deployment Destination </h2>

- <b>Azure Kubernetes Cluster</b> 

<h2>Project walk-through:</h2>

<p align="center">

create a VM with Ubuntu 20.04, install Docker and Docker Compose <br/>

<img width="450" alt="Picture1" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/010f520f-72a7-4217-9ba3-bb3d4472d4e5">

<br />
<br />

Create Azure container registry (ACR) and capture details for futher use. <br/>

<img width="450" alt="Picture2" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/785a119a-0530-4d81-9a5e-3c734daa688e">
<br />
<br />

Create an Azure Kurbenetes Cluster (AKS). <br/>

<img width="450" alt="Picture3" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/58433d13-3a2e-4732-81c7-ea91109045b9">
<br />
<br />

Clone Git repository <br/>

<img width="450" alt="Picture4" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/cdd597eb-86dd-4ee1-94eb-d989c9aad48a">

<br />
<br />

Build the Docker image <br/>

<img width="450" alt="Picture5" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/7ba2ad27-f586-46b8-9e43-00ad48a2756e">

<br />
<br />

Create an EC2 instance where the website will be deployed. (attach an IAM role to the EC2 to 
Access S3, install a code deploy agent on EC2)
 <br/>

<img width="450" alt="step 6" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/3e8acb66-5f18-477a-97a9-c10d4f156a49"/>


<br />
<br />

Install codedeploy agent on EC2 <br/>

<img width="450" alt="step 7" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/2c0df345-cffb-4f02-8cdf-c160f0506bd7"/>


<br />
<br />

Create a deployment application using code deploy <br/>

<img width="450" alt="step 8" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/c564f140-833b-4f4a-94f5-af38d5b535ef"/>


<br />
<br />


Create deployment group (attach a code deploy service role here) <br/>

<img width="450" alt="step 9" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/46243881-6a92-4aed-8083-06c3dbd857ea"/>

<br />
<br />

Create a deployment. (code deploy only supports s3 or GitHub repos not code-commit) <br/>

<img width="450" alt="step 10" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/15904486-9146-48dd-a07d-7a235059e69b"/>


<br />
<br />

Automate the entire deployment process using Codepipeline <br/>

<img width="450" alt="step 11" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/f7e6dae7-11c6-440c-ba1d-d9f825e8b1df"/>

<br />
<br />


The build process <br/>

<img width="450" alt="step 12" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/3b43467c-43c5-45c5-a52a-8784ca8d3ff2"/>


<br />
<br />

The deployment process <br/>

<img width="450" alt="step 13" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/3dc6423c-f224-438b-8845-e79ac4eb218d"/>


<br />
<br />

Viola!!! the end product <br/>

<img width="450" alt="step 14" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/9cad995f-5b76-4dde-9024-79ead58315b4"/>

<br />
<br />

<!--






