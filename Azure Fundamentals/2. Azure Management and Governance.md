# Azure Management and Governance
<b>Via Microsoft Learn</b>
## Cost Affecting factors
1) <b>Resource Type:</b> With a storage account, you specify a type such as blob, a performance tier, an access tier, redundancy settings, and a region. Creating the same storage account in different regions may show different costs and changing any of the settings may also impact the price.
2) <b>Consumption:</b> Pay-as-you-go has been a consistent theme throughout, and that’s the cloud payment model where you pay for the resources that you use during a billing cycle. If you use more compute this cycle, you pay more. If you use less in the current cycle, you pay less. It’s a straight forward pricing mechanism that allows for maximum flexibility.
3) <b>Geography</b>
4) <b>Maintainance:</b> By keeping an eye on your resources and making sure you’re not keeping around resources that are no longer needed, you can help control cloud costs.
5) <b>Network Traffic</b> 

## Calculation of Cost
### Pricing Calculator
With the pricing calculator, you can estimate the cost of any provisioned resources, including compute, storage, and associated network costs. You can even account for different storage options like storage type, access tier, and redundancy.
### TCO Calculator (Total Cost of Ownership)
With the TCO calculator, you enter your configuration, add in assumptions like power and IT labor costs, and are presented with an estimation of the cost difference to run the same environment in your current datacenter or in Azure.
<br><br>
<b>The main difference is that the Azure Pricing Calculator estimates costs for specific Azure services based on user configurations, while the TCO Calculator compares the total costs of running workloads on-premises versus in Azure to highlight potential savings from migration.</b>

## Tags
<ul>
<li>Resource management Tags enable you to locate and act on resources that are associated with specific workloads, environments, business units, and owners.</li>
<li>Cost management and optimization Tags enable you to group resources so that you can report on costs, allocate internal cost centers, track budgets, and forecast estimated cost.</li>
<li>Operations management Tags enable you to group resources according to how critical their availability is to your business. This grouping helps you formulate service-level agreements (SLAs). An SLA is an uptime or performance guarantee between you and your users.</li>
<li>Security Tags enable you to classify data by its security level, such as public or confidential.</li>
<li>Governance and regulatory compliance Tags enable you to identify resources that align with governance or regulatory compliance requirements, such as ISO 27001. Tags can also be part of your standards enforcement efforts. For example, you might require that all resources be tagged with an owner or department name.</li>
<li>Workload optimization and automation Tags can help you visualize all of the resources that participate in complex deployments. For example, you might tag a resource with its associated workload or application name and use software such as Azure DevOps to perform automated tasks on those resources.</li>
  
  ## Microsoft Purview
  Microsoft Purview brings insights about your on-premises, multicloud, and software-as-a-service data together.
  Microsoft Purview, by managing and monitoring your data, is able to help your organization:
<ul>
<li>Protect sensitive data across clouds, apps, and devices.</li>
<li>Identify data risks and manage regulatory compliance requirements.</li>
<li>Get started with regulatory compliance.</li>
</ul>

## Azure Policy
Azure Policy enables you to define both individual policies and groups of related policies, known as initiatives. Azure Policies can be set at each level, enabling you to set policies on a specific resource, resource group, subscription, and so on. Additionally, Azure Policies are inherited. Azure Policy comes with built-in policy and initiative definitions for Storage, Networking, Compute, Security Center, and Monitoring. 
Azure Policy enables you to define both individual policies and groups of related policies, known as initiatives. Azure Policies can be set at each level, enabling you to set policies on a specific resource, resource group, subscription, and so on. Additionally, Azure Policies are inherited. Azure Policy comes with built-in policy and initiative definitions for Storage, Networking, Compute, Security Center, and Monitoring. 

## Resource Locks
A resource lock prevents resources from being accidentally deleted or changed. 
<br>Delete means authorized users can still read and modify a resource, but they can't delete the resource.<br>ReadOnly means authorized users can read a resource, but they can't delete or update the resource. Applying this lock is similar to restricting all authorized users to the permissions granted by the Reader role.

## Interacting with Azure

### Azure Portal
The Azure portal is a web-based, unified console that provides an alternative to command-line tools. With the Azure portal, you can manage your Azure subscription by using a graphical user interface. Azure Cloud Shell is a browser-based shell tool that allows you to create, configure, and manage Azure resources using a shell. Azure Cloud Shell support both Azure PowerShell and the Azure Command Line Interface (CLI), which is a Bash shell.
### Azure CLI (Command Line Interface)
The Azure CLI is functionally equivalent to Azure PowerShell, with the primary difference being the syntax of commands. While Azure PowerShell uses PowerShell commands, the Azure CLI uses Bash commands.
### Azure PowerShell
Azure PowerShell is a shell with which developers, DevOps, and IT professionals can run commands called command-lets (cmdlets). These commands call the Azure REST API to perform management tasks in Azure. Cmdlets can be run independently to handle one-off changes, or they may be combined to help orchestrate complex actions.
## Azure ARM (Azure Resource Manager)
Azure Resource Manager (ARM) is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. Anytime you do anything with your Azure resources, ARM is involved.
### Key Features of ARM Templates

- **Declarative Syntax**: 
  - Allows for the creation and deployment of Azure infrastructure by specifying desired resources without writing programming commands or deployment sequences.

- **Repeatable Results**: 
  - Enables consistent deployment of infrastructure across the development lifecycle using the same ARM template for multiple dev/test environments.

- **Orchestration**: 
  - Azure Resource Manager manages the order of resource deployment, creating interdependent resources correctly and deploying them in parallel when possible, resulting in faster deployments through a single command.

- **Modular Files**: 
  - Supports breaking templates into smaller, reusable components that can be linked together during deployment, including nesting templates for consistent deployment of complex environments.

- **Extensibility**: 
  - Allows the inclusion of PowerShell or Bash scripts within ARM templates, enhancing resource setup capabilities, with scripts either embedded or referenced from external sources for complete environment setup.

## Bicep
Bicep is a language that uses declarative syntax to deploy Azure resources. A Bicep file defines the infrastructure and configuration. Then, ARM deploys that environment based on your Bicep file. While similar to an ARM template, which is written in JSON, Bicep files tend to use a simpler, more concise style.
- **Easy to Read**: It has a simpler and cleaner syntax than traditional JSON templates, making it easier to write and understand.

- **Declarative**: You describe what you want to create, and Bicep takes care of the details of how to do it.

- **Reusable**: You can create modules (small pieces of code) that can be reused in different projects.

- **Type Safety**: Bicep checks for errors as you write, helping you catch mistakes early.

- **Works with Azure**: It integrates directly with Azure Resource Manager, allowing you to deploy resources easily.

- **No State Management**: Bicep doesn’t keep track of the state of resources; Azure does that for you.

## Azure Advisor
Azure Advisor evaluates your Azure resources and makes recommendations to help improve reliability, security, and performance, achieve operational excellence, and reduce costs. Azure Advisor is designed to help you save time on cloud optimization. The recommendation service includes suggested actions you can take right away, postpone, or dismiss.

## Azure Monitor
Azure Monitor is a platform for collecting data on your resources, analyzing that data, visualizing the information, and even acting on the results. Azure Monitor can monitor Azure resources, your on-premises resources, and even multi-cloud resources like virtual machines hosted with a different cloud provider.
### Azure Log Analytics
Azure Log Analytics is the tool in the Azure portal where you’ll write and run log queries on the data gathered by Azure Monitor.
### Azure Monitor Alerts
Azure Monitor Alerts are an automated way to stay informed when Azure Monitor detects a threshold being crossed. You set the alert conditions, the notification actions, and then Azure Monitor Alerts notifies when an alert is triggered. Depending on your configuration, Azure Monitor Alerts can also attempt corrective action.
### Application Insights
Application Insights, an Azure Monitor feature, monitors your web applications. Application Insights is capable of monitoring applications that are running in Azure, on-premises, or in a different cloud environment.
