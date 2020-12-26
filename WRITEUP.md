# Write-up Template

## Analyze, choose, and justify the appropriate resource option for deploying the app.

##*For **both** a VM or App Service solution for the CMS app:*
## *Analyze costs, scalability, availability, and workflow*

### VM
- Costs: Virtual Machines are more expensive than App Services, in the other hand, You have control over the VM, so you
  can stop the VM to avoid charges in case you app or services are not running.
- Scalability & Availability: Multiple VMs can be grouped to provide high scalability and availability.
  For Scaling there are two options: Virtual Machine Scale Sets and Load Balancers.
- Workflow: create or utilize a resource group, create a VM, connect to the VM, install app dependencies, run the application

### App Service
- Costs: App Services are cheaper than VMs, in the other hand, you’re always paying for the service plan, even if your services 
  or application isn’t running.
- Scalability: App service provided vertical (increases or decreases resources like amount of CPU or RAM until a maximum
  of 14 GB of memory and 4 vCPU cores instance) and horizontal (increases or decreases VM instances) scaling.
- Availability: App service provides high availability
  and support for both Linux and Windows environments.
- Workflow: create or utilize a resource group, create the App service, deploy the code(app) to the app service.

### *Choose the appropriate solution (VM or App Service) for deploying the app*
- The appropriate solution for deploying this app is an App Service

### *Justify your choice*

App Service is a better option than Vm because:
- Cost in general is less expensive than VMs.
- There is not need for control of the underlying operating system or any custom software is needed to be installed.
- This application is a lightweight, so no need for high performance compute services.
- Availability and scalability are provided, so considering this is a lightweight application, 
  vertical limitations in an App Service is ok.
  
## Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
Some needs have to appear in order to change from App service to VM like:
- More features will be added to the application.
- A huge demand is needed in a way that vertical scaling limitations are exceeded.
- The need for a custom software (OS, third party software, etc.) to be installed.
- Specific OS settings needed to be modified or implemented that requires further control of the OS on which the app is running.

