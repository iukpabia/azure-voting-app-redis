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

Confirm image build on the designated port number on browser <br/>

<img width="450" alt="Picture6" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/7ec23259-d6db-425e-b6d2-e8ba0d4ae7be">


<br />
<br />

Tag image <br/>

<img width="450" alt="Picture7" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/94e394cc-253b-43be-ac99-d1489645a758">

<br />
<br />

Push Tagged image to Azure Container Registry (ACR) <br/>

<img width="465" alt="Picture8" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/2ee4c001-3119-4ceb-862f-27efed83347f">



<br />
<br />


Deploy application to Azure Kurbenetes Cluster (AKS) <br/>

<img width="450" alt="Picture9" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/b739e76f-ae59-4f1a-b16f-ac022242ae74">
<br />
<br />

 Confirm application is working <br/>

<img width="450" alt="Picture10" src="https://github.com/iukpabia/AWS-CI-CD-Website-Deployment/assets/127888235/73c8144d-f5ce-4f3f-84d7-60d912dc7ac7">

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






