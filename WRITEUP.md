# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

## Comparison of VM or App Service
### Virtual Machines
Azure Virtual Machines (VMs) provide infrastructure as a service (IaaS) by allowing you to create and use virtual machines in the cloud.

Benefits of VMs:
* VMs gives you full access and control of the VM.
* Lower up-front cost compared to purchasing and maintaining hardware.
* Support of both Linux and Windows VMs.
* Multiple types to choose from, such as compute or memory-optimized VMs, along with varying amounts of CPU, RAM and storage.
* VMs allow for the installation of custom images and are an excellent choice for migrating from an on-premises server to the cloud.
* Multiple VMs can be grouped to provide high availability, scalability, and redundancy.

Limitations of VMs:
* VMs are more expensive
* They are more time consuming to set up and maintain

### App Service
Azure App Service is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends. It is a Platform as a Service (PaaS) that allows a developer to focus on the application while Azure takes care of the infrastructure.
* Benefits of App Service:
* Support of multiple languages, such as .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python
* High availability, auto-scaling and support of both Linux and Windows environments.
* Continuous deployment model using GitHub, Azure DevOps, or any Git repo.
* Vertical or Horizontal scaling. 

Limitations of App Service:
* You have limited access to the host server, so you are unable to control the underlying OS or install software on the server.
* You’re always paying for the service plan, even if your services or application isn’t running.
* There are hardware limitations, such as a maximum of 14GB of memory and 4 vCPU cores per instance
* While they support multiple languages, as noted in the benefits above, they are limited to just using those languages (as of when this course was built).

There are specific use cases that either App Service or VMs would fit.
* Virtual Machines are usually better when you need control of the underlying operating system or are using custom software to support your needs.

* App Service is typically better for lightweight applications and services like this Article CMS application, especially since I don't have the need for high performance compute services and App Service supports Python as a development language. Also, it is relatively cheaper and easier to set up and manage than VMs.