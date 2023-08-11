# Azure Governance and Complaint 

## Managing Subscriptions 

#### What is an Azure Subscription 
An Azure subscription is a logical container used to provision related business or technical resources in Azure. It holds the details of all your resources like virtual machines (VMs), databases, and more. When you create an Azure resource like a VM, you identify the subscription it belongs to.   

Subscriptions are the biling unit that aggregates all costs of underlying resouces . 
subscriptions contain resouce groups and their assocaited resouces 

### Types of Subscription 
* Azure Plan 
* Enterpriese Agreement Support 
* Microsoft Azure EA Sponsorship 
* Pay As you Go 
* Support Plans 
* Free trail 
* Visual Studio Professional Subsciber 
* Visual Test Professioal Subscriber 
* MSDN Platforms subscibers 
* Visual Studio Enterprise subscribers 
* Visual Studio Enterprise (BizSpark) Subscription 


### Subscription Naming Conventions 

1. Prod/Dev/Staging 
Subscription are named based on whether they are production, development, or stating enviroments 

2. Department/Teams 
Subsciprtions are named based on the Department or team the subscription is intended for so that billing can then be easily assocaited with a given business unit 

3. Region 
Subscription are name based on the region of the business that uses the subscription


## Using Management Group 

Organize and manage subscription by logically grouping them into Management groups

#### Benefits of Management Groups 
* Organizational Hierarchy 
* Provides another Scope for enforcing Governance and compliance 

### Understainding Azure Policy 
An Azure Policy definition, created in Azure Policy, is a rule about specific security conditions that you want controlled. Built in definitions include things like controlling what type of resources can be deployed or enforcing the use of tags on all resources.

Enforcing and Enable Auditin . 

### Componnets of a Policy 
* Policy Definition 
Defines the evaluation criteria for compliance, and defines the actions that take place, Either audit or deny should be something outside of compliance 

* Policy Assignment 
The scope at which we will assign our policy, The scope could be a management group, subscription, resouce group or resouce. 

* Initiative Definition 
A collection of policies that are4 tailored to achieving a singular high-level goal together (e.g, ensuring that VMs meet standards )

### Tagging Resources 
Tags are metadata elements that you apply to your Azure resources. They're key-value pairs that help you identify resources based on settings that are relevant to your organization. If you want to track the deployment environment for your resources, add a key named Environment 

### Locks in Azure 
As an administrator, you can lock an Azure subscription, resource group, or resource to protect them from accidental user deletions and modifications. The lock overrides any user permissions. You can set locks that prevent either deletions or modifications. In the portal, these locks are called Delete and Read-only

### Lock Types 
* Read only allows authorized users to read a resource , but they cannot delete or update the resource 

* Can NotDelete allows authorized users to read and modify a resouce , but they cannot delete the resouce  