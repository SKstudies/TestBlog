# <a href="https://blogappfrt.azurewebsites.net//">Efficient CI/CD Pipeline for Azure Web App Deployment.</a>

### Links : 
Synopsis With Screenshots: https://drive.google.com/file/d/1VpGv8THzEndNsOxpTU52o2T0VFpj8qXg/view?usp=sharing

Demo Video + Template: https://drive.google.com/drive/folders/11buUUOqcWXjfAOalLgWIdtyAGVJizOOC?usp=drive_link

ProjectURL: https://azureproject.cloud/  

Default Domain: https://blogappfrt.azurewebsites.net/

(message from developer: if website url is not working then app service is stopped due to expired subscription you can still watch the demo video)


### Industry :
ED-Tech


### Project Title :
Efficient CI/CD Pipeline for Azure Web App Deployment.


### Overview :
The project focuses on solving the problem of manual and error-prone deployment processes for web applications on the Azure platform. It addresses the need for a streamlined, efficient, and reliable deployment workflow.

Core Features:
Continuous Integration and Continuous Deployment (CI/CD): The project implements a robust CI/CD pipeline that automates the deployment process. Developers push code changes to a GitHub repository, triggering a series of automated actions that build a Docker container of the web application, store it in an Azure Container Registry (ACR), and deploy it to an Azure App Service.

Azure Services Utilized:
1.	Azure Container Registry (ACR): Used for storing and version-controlling Docker container images.
2.	Azure App Service: The platform where the web application is hosted.
3.	Azure DevOps Integration: Azure DevOps is used to set up the build and release pipelines, ensuring the seamless automation of the CI/CD process.
4.	Custom Domain: The project enables access to the web application via a custom domain, mapping a custom domain name to app service and using App Service Managed Certificate.

The project's purpose is to streamline web application deployment on Azure, making it more efficient, reliable, and error-free. It offers developers a solution that minimizes manual deployment efforts, accelerates the release cycle, and ensures consistent and hassle-free updates and new feature deployments. The integration of multiple Azure services and DevOps practices makes this project a powerful and comprehensive solution for Azure-based web application deployment.


### Flow Diagram:
<a href="https://futurereadytalent.in/"><p align= "center"><img src="https://github.com/SKstudies/Blogs/blob/master/media/Picture4.png"></p></a> 

### Expaination: 
This project involves creating a seamless deployment pipeline for a web application. It leverages Microsoft Azure services, including Azure Container Registry (ACR), Azure App Service, and Azure DevOps. Here's a breakdown of the key components and steps:
1.	Azure Container Registry (ACR): An ACR repository is set up to store Docker containers of the web application. It will store the containers created by build pipeline.
2.	GitHub Repository: The project code is stored in a GitHub repository, providing version control and collaboration capabilities.
3.	Azure DevOps: Azure DevOps is utilized to automate the build and release processes.
4.	Build Pipeline: A build pipeline is created in Azure DevOps, which compiles the project code from the GitHub repository, packages it into a Docker container, and stores the container in ACR.
5.	Azure App Service: An Azure App Service is configured to host the web application using Docker containers. This service provides a scalable and cost-effective hosting solution, as per the requirement I will not be using auto scaling.
6.	Deployment Center: The deployment center is accessed from the Azure portal it is the part of App Service from where I can manually deploy the container stored in ACR on the App Service.
7.	Release Pipeline: A release pipeline in Azure DevOps automates the deployment of the web application. Whenever changes are committed to the master branch in GitHub, the build and release processes are triggered automatically.

By automating these processes, the project enhances efficiency, reduces human errors, and allows for easy scaling and continuous integration. The project serves as a model for streamlined web application deployment using Azure services.


### Problem Statement :
The project aims to address the challenge of manual and error-prone deployment processes for web applications on the Azure platform. Inefficient deployment practices often result in delays and issues in delivering updates and new features to end-users. This project identifies the problem of manual deployment and seeks to solve it through the implementation of a streamlined Continuous Integration and Continuous Deployment (CI/CD) pipeline. By automating the deployment process, the project mitigates deployment errors, enhances delivery speed, and promotes a more reliable and efficient web application deployment on Azure. This addresses the existing problem of manual and error-prone deployments and offers an opportunity to significantly improve the deployment workflow for web applications hosted on Azure.

### Project Description :
The core idea behind this project is to address the problem of manual and error-prone deployment processes for web applications on the Azure platform. We are leveraging Azure's robust feature set to create an automated Continuous Integration and Continuous Deployment (CI/CD) pipeline. This project targets developers and development teams looking to streamline their web application deployment on Azure.

The problem we are solving is the inefficiency of manual deployments, which often lead to delays, errors, and inconsistencies in the release of updates and new features. By implementing an automated CI/CD pipeline, we are mitigating this problem. Our project allows developers to push their code changes to a GitHub repository, and from there, Azure DevOps takes over. It builds a Docker container of the web application, stores it in an Azure Container Registry (ACR), and then deploys it to an Azure App Service. This automated pipeline ensures that the deployment process is error-free and rapid.

Our project addresses the clear need for efficient, reliable, and consistent web application deployment on Azure. By automating the process, it not only eliminates manual errors but also accelerates the release cycle. The purpose and basic functionality of our project are closely aligned with the problem statement, offering a systematic solution that enables developers to focus on coding while the CI/CD pipeline takes care of deployment intricacies.



### Primary Azure Technology :
1.	Azure Container Registry (ACR): ACR is the foundation for storing Docker container images, enabling us to efficiently manage and distribute containerized applications. We use ACR to store and version control our application's container images.
2.	Azure App Service: Azure App Service is the platform where we host and run our web application. It provides a managed environment for web app deployment, including auto-scaling, load balancing, and seamless integration with our Docker containers stored in ACR.


### Other Azure Technologies :
1.	Azure DevOps: While not a core Azure service, Azure DevOps plays a crucial role in this project. It is used for setting up the build and release pipelines, automating the CI/CD process, and connecting various components of the project together.
2.	DNS (for Custom Domain): The project enables access to the web application via a custom domain, mapping a custom domain name to app service and using App Service Managed Certificate.
3.	App Service Managed Certificate: Providing SSL certificates for secure communication with the custom domain

### Complete Step By Step Process :
1. Create Container Repository:
![Alt text](<media/Process Screenshots/Screenshot (528).png>)
![Alt text](<media/Process Screenshots/Screenshot (529).png>)
![Alt text](<media/Process Screenshots/Screenshot (530).png>)

2. Use Azure Devops Portal For Creating Service Connections From Devops To Github and ACR.
![Alt text](<media/Process Screenshots/Screenshot (531).png>)
![Alt text](<media/Process Screenshots/Screenshot (532).png>)
![Alt text](<media/Process Screenshots/Screenshot (533).png>)
![Alt text](<media/Process Screenshots/Screenshot (534).png>)
![Alt text](<media/Process Screenshots/Screenshot (535).png>)
![Alt text](<media/Process Screenshots/Screenshot (536).png>)
![Alt text](<media/Process Screenshots/Screenshot (537).png>)
![Alt text](<media/Process Screenshots/Screenshot (538).png>)
![Alt text](<media/Process Screenshots/Screenshot (539).png>)

3. Push The Code To Github Repo Which Should Contain the Required Docker File.
![Alt text](<media/Process Screenshots/Screenshot (540).png>)
![Alt text](<media/Process Screenshots/Screenshot (541).png>)

4. Create Build Pipeline To Create And Store The Docker Container In ACR.
![Alt text](<media/Process Screenshots/Screenshot (543).png>)
![Alt text](<media/Process Screenshots/Screenshot (544).png>)
![Alt text](<media/Process Screenshots/Screenshot (545).png>)
![Alt text](<media/Process Screenshots/Screenshot (546).png>)
![Alt text](<media/Process Screenshots/Screenshot (547).png>)
![Alt text](<media/Process Screenshots/Screenshot (548).png>)
![Alt text](<media/Process Screenshots/Screenshot (549).png>)
![Alt text](<media/Process Screenshots/Screenshot (550).png>)
![Alt text](<media/Process Screenshots/Screenshot (551).png>)
![Alt text](<media/Process Screenshots/Screenshot (552).png>)
![Alt text](<media/Process Screenshots/Screenshot (553).png>)

5. Docker Container Stored In The Repository.
![Alt text](<media/Process Screenshots/Screenshot (554).png>)

6. Allow Access. 
![Alt text](<media/Process Screenshots/Screenshot (555).png>)

7. Create Web App.
![Alt text](<media/Process Screenshots/Screenshot (587).png>)
![Alt text](<media/Process Screenshots/Screenshot (588).png>)
![Alt text](<media/Process Screenshots/Screenshot (589).png>)
![Alt text](<media/Process Screenshots/Screenshot (591).png>)
![Alt text](<media/Process Screenshots/Screenshot (592).png>)

8. Establish The Required Environment And Deploy.
![Alt text](<media/Process Screenshots/Screenshot (593).png>)
![Alt text](<media/Process Screenshots/Screenshot (594).png>)
![Alt text](<media/Process Screenshots/Screenshot (595).png>)
![Alt text](<media/Process Screenshots/Screenshot (596).png>)
![Alt text](<media/Process Screenshots/Screenshot (597).png>)
![Alt text](<media/Process Screenshots/Screenshot (598).png>)

9. Create Release Pipeline.
![Alt text](<media/Process Screenshots/Screenshot (599).png>)
![Alt text](<media/Process Screenshots/Screenshot (600).png>)
![Alt text](<media/Process Screenshots/Screenshot (601).png>)
![Alt text](<media/Process Screenshots/Screenshot (602).png>)
![Alt text](<media/Process Screenshots/Screenshot (603).png>)
![Alt text](<media/Process Screenshots/Screenshot (604).png>)
![Alt text](<media/Process Screenshots/Screenshot (605).png>)
![Alt text](<media/Process Screenshots/Screenshot (606).png>)
![Alt text](<media/Process Screenshots/Screenshot (607).png>)
![Alt text](<media/Process Screenshots/Screenshot (608).png>)
![Alt text](<media/Process Screenshots/Screenshot (609).png>)
![Alt text](<media/Process Screenshots/Screenshot (610).png>)

10. Search Default Domain If Website Is Running.
![Alt text](<media/Process Screenshots/Screenshot (611).png>)

11. Create Custom Domain Scale Up The Plan AS Free Plan Does Not Support Custom Domain.
![Alt text](<media/Process Screenshots/Screenshot (612).png>)
![Alt text](<media/Process Screenshots/Screenshot (613).png>)
![Alt text](<media/Process Screenshots/Screenshot (614).png>)

12. Add A Custom Domain With App Service Managed Certificate.
![Alt text](<media/Process Screenshots/Screenshot (623).png>)
![Alt text](<media/Process Screenshots/Screenshot (624).png>)
![Alt text](<media/Process Screenshots/Screenshots.png>)
![Alt text](<media/Process Screenshots/Screenshots1.png>)
![Alt text](<media/Process Screenshots/Screenshots0.png>)
![Alt text](<media/Process Screenshots/Screenshots2.png>)

#### CICD pipeline in action
13. Commit Changes To github.
![Alt text](<media/Process Screenshots/Screenshots3.png>)


14. Build Pipline Triggered
![Alt text](<media/Process Screenshots/Screenshots4.png>)

15. Containers Created In ACR.
![Alt text](<media/Process Screenshots/Screenshots5.png>)

16. Release Pipeline Triggered.
![Alt text](<media/Process Screenshots/Screenshots6.png>)

17. Successful Deployment On App Service.
![Alt text](<media/Process Screenshots/Screenshots7.png>)

18. Site is Running.
![Alt text](<media/Process Screenshots/Screenshots8.png>)





<a href="https://futurereadytalent.in/"><p align= "center"><img src="https://github.com/ROHAN0011/Microsoft-Future-Ready-Talent-Internship-Project/blob/5ae1e52f4f4236d8ca92ea9189794835ce087467/FRT.jpeg" width="700" height= "350"></p></a>  


