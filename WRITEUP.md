# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

- Azure Virtual Machines (VMs) provide infrastructure as a service (IaaS) by allowing you to create and use virtual machines in the cloud. For VM there is lower upfront cost since we don't have to purchase and maintain hardware. VM supports both Windows and Linux. VM is an excellent option for testing and deployment because you can quickly spin up different operating systems and application configuration. You can quickly tear down when you no longer need it. Multiple VMs can be grouped to provide high availability, scalability, and redundancy. VMs are an excellent choice for migrating from an on-premises server to the cloud.
There are various types to choose from, such as compute or memory-optimized VMs, along with varying amounts of CPU, RAM and storage.

- Azure App Service is a Platform as a Service (PaaS) that allows a developer to focus on the application while Azure takes care of the infrastructure. App Service is an excellent choice for deploying lightweight application or services. It supports multiple languages, such as .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python. It provides high availability and auto-scaling. It also supports both Windows and Linux and continuous deployment model using GitHub, Azure DevOps, or any Git repo. App Service can scale vertically or horizontally. Vertical scaling increases or decreases resources allocated to our App Service, such as the amount of vCPUs or RAM, by changing the App Service pricing tier. Horizontal scaling increases or decreases the number of Virtual Machine instances our App Service is running.
You can set the amount of hardware allocated to host your application, and cost varies based on the plan you choose. There are three different tiers - Dev/Test, Production, and Isolated. 

- Virtual Machines are usually better when we need control of the underlying operating system or are using custom software to support our needs; an app service is typically better for lightweight applications and services, especially when we don't have the need for high performance compute services. App Service has hardware limitations, such as a maximum of 14GB of memory and 4 vCPU cores per instance.
Therefore, for the purpose of the FlaskWebProject I am choosing App Service since it's a lightweight application and we don't have the need for high performance compute services. And we can use the free option within Dev/Test for the exercise with App Service while VMs tend to be more expensive.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

If I need a full control over the underlying operating system and software or more computing resources beyond the App Service (limit of 14GB and 4 vCPU cores) then we'll have to switch to VM.
