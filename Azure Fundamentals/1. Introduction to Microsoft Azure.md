# Introduction to Microsoft Azure 
<b>Via Microsoft Learn </b>

## What is Microsoft Azure?
Azure has simple web services for hosting your business presence in the cloud. Azure also supports running fully virtualized computers managing your custom software solutions. Azure provides a wealth of cloud-based services like remote storage, database hosting, and centralized account management. Azure also offers new capabilities like artificial intelligence (AI) and Internet of Things (IoT) focused services.

### About Cloud Computing
Cloud computing is the delivery of computing services over the internet. Computing services include common IT infrastructure such as virtual machines, storage, databases, and networking. Cloud services also expand the traditional IT offerings to include things like Internet of Things (IoT), machine learning (ML), and artificial intelligence (AI).

### Shared Responsiblity Model
When using a cloud provider, you are responsible for the information and data stored in the cloud, the devices that connect to it, and the accounts and identities of users and services within your organization. Conversely, the cloud provider is responsible for the physical datacenter, network, and hosts. Your specific service model will dictate the division of responsibility for aspects like operating systems, network controls, applications, and identity management.<br>
<br><b>IaaS (Infrastructure as a Service):</b>
The cloud provider is responsible for the foundational infrastructure, like storage, virtual machines, and networks. The customer is responsible for everything built on the infrastructure, like the operating system, applications, runtime, and data. 
<br><b>PaaS (Platform as a Service):</b>
A middle ground between IaaS and SaaS, PaaS distributes responsibility evenly between the cloud provider and the customer. 
</br><b>SaaS (Software as a Service):</b>
The cloud provider is responsible for the entire infrastructure and applications, while the customer is responsible for managing data and user access/identity permissions. 

### Cloud Models
There are three main cloud models: public, private, and hybrid. Public clouds are owned and operated by a single entity. A public cloud is built, controlled, and maintained by a third-party cloud provider. With a public cloud, anyone that wants to purchase cloud services can access and use resources. A hybrid cloud is a computing environment that uses both public and private clouds in an inter-connected environment. A hybrid cloud environment can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources. Hybrid cloud can be used to provide an extra layer of security. For example, users can flexibly choose which services to keep in public cloud and which to deploy to their private cloud infrastructure.

<b> Azure Arc: </b>Azure Arc is a set of technologies that helps manage your cloud environment. Azure Arc can help manage your cloud environment, whether it's a public cloud solely on Azure, a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment running on multiple cloud providers at once. Servers, Kubernetes clusters, Azure data services.SQL Server,Virtual machines (preview.)

### Capital Expenditure (CapEx) and Operational Expenditure (OpEx)
CapEx is typically a one-time, up-front expenditure to purchase or secure tangible resources. A new building, repaving the parking lot, building a datacenter, or buying a company vehicle are examples of CapEx.<br>In contrast, OpEx is spending money on services or products over time. Renting a convention center, leasing a company vehicle, or signing up for cloud services are all examples of OpEx.<br>Cloud computing falls under OpEx because cloud computing operates on a consumption-based model. With cloud computing, you don’t pay for the physical infrastructure, the electricity, the security, or anything else associated with maintaining a datacenter. Instead, you pay for the IT resources you use.</br><b> Cloud computing is a way to rent compute power and storage from someone else’s datacenter. You can treat cloud resources like you would resources in your own datacenter. However, unlike in your own datacenter, when you're done using cloud resources, you give them back. You’re billed only for what you use.</b>

## Benefits of Cloud Computing
### Scalibility
 Scalability refers to the ability to adjust resources to meet demand. If you suddenly experience peak traffic and your systems are overwhelmed, the ability to scale means you can add more resources to better handle the increased demand.

The other benefit of scalability is that you aren't overpaying for services. Because the cloud is a consumption-based model, you only pay for what you use. If demand drops off, you can reduce your resources and thereby reduce your costs.

Scaling generally comes in two varieties: vertical and horizontal. Vertical scaling is focused on increasing or decreasing the capabilities of resources. Horizontal scaling is adding or subtracting the number of resources.

### Reliability
Reliability is the ability of a system to recover from failures and continue to function. It's also one of the pillars of the Microsoft Azure Well-Architected Framework. With this global scale, even if one region has a catastrophic event other regions are still up and running.
### Predictibility
### Performance
Autoscaling, load balancing, and high availability are just some of the cloud concepts that support performance predictability. If you suddenly need more resources, autoscaling can deploy additional resources to meet the demand, and then scale back when the demand drops. Or if the traffic is heavily focused on one area, load balancing will help redirect some of the overload to less stressed areas.
### Cost
By operating in the cloud and using cloud analytics and information, you can predict future costs and adjust your resources as needed. You can even use tools like the Total Cost of Ownership (TCO) or Pricing Calculator to get an estimate of potential cloud spend.

## Management of the Cloud
### Cloud Management
Management of the cloud speaks to managing your cloud resources. In the cloud, you can:
<ul>
<li>Automatically scale resource deployment based on need.</li>
<li>Deploy resources based on a preconfigured template, removing the need for manual configuration.</li>
<li> Monitor the health of resources and automatically replace failing resources.</li>
<li>Receive automatic alerts based on configured metrics, so you’re aware of performance in real time.</li>
</ul>
You can manage these through a Web Portal, Using comman line interface, APIs, or PowerShell.