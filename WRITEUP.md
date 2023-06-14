## Analyze, choose, and justify the appropriate resource option for deploying the app.

#### App Service:
Azure WebApps is a fast and simple way to create web apps. it has build-in CI/CD integration and has zero downtime deployments. complexity level is less which makes it easier to manage and also less in cost compared to VM. App Service costs less.
| Service  | Cost (Per Month)  |
| :------------ |:---------------|
| App Service     | $55 |
| Storage account     | $22 |
| SQL Database cost | $370 |

#### Virtual Machines:
Azure Virtual Machines let us provision Windows or Linux VMs in seconds, can be deployed with own VM image or images from the Azure Marketplace, ability to scale from one to thousands of VM instances in minutes with Azure Virtual Machine Scale Sets. Virtual Machines costs more.
| Service  | Cost (Per Month)  |
| :------------ |:---------------|
| Virtual Machine     | $150 |
| Storage account     | $22 |
| SQL Database cost | $370 |

As our application is light and not much control is required. So concerning the costs and complexity level of the service I chose App Service.

### Assess app changes that would change your decision.

As our application is a not business critical and doesn't require any special control over the deployment, I used App Service. In the future I might add more functionality to the app and we might require better control over the deployment or decide to write business critical articles or ultimate usage of the app might increase. In that case I would migrate to Virtual Machines and use Higher Tier SQL database for better access and security. New Plan will be according to the budget threshold.
