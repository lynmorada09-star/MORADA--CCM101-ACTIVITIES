# Cloud Provider Comparison
 Comparison of Core Infrastructure Services

In the previous checkpoints, I investigated a Linux environment using
KillerCoda. The environment had an Intel Xeon E312xx (Sandy Bridge, IBRS
update) CPU, 1 CPU core, 1.9 GiB of RAM, a 20 GB virtual disk, and a network
interface with the IP address 172.30.1.2/24. The operating system was Ubuntu
24.04.4 LTS with kernel version 6.8.0-136-generic.

These observations helped identify compute, storage, and networking as major
cloud infrastructure components. The following table compares these
infrastructure components with equivalent services offered by AWS, Microsoft
Azure, and Google Cloud Platform.

| Infrastructure Component | AWS | Microsoft Azure | Google Cloud Platform |
|---|---|---|---|
| Compute | Amazon EC2 | Azure Virtual Machines | Google Compute Engine |
| Storage | Amazon S3 | Azure Blob Storage | Google Cloud Storage |
| Networking | Amazon VPC | Azure Virtual Network (VNet) | Google Cloud VPC |
| Identity and Access Management (IAM) | AWS IAM | Microsoft Entra ID / Azure RBAC | Google Cloud IAM |

## Guide Questions

### 1. Which cloud provider offers the broadest range of services? Explain your answer.

AWS offers one of the broadest selections of cloud services. Like the
KillerCoda environment where compute, storage, and networking resources were
observed separately, AWS provides services for these areas along with many
other cloud technologies.

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

I would recommend Microsoft Azure for an organization that primarily uses
Microsoft products. Azure provides services such as Azure Virtual Machines,
Azure Blob Storage, Azure Virtual Network, and Microsoft identity and access
services that can work closely with Microsoft technologies.

### 3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?

Google Cloud is widely recognized for its strengths in Artificial
Intelligence, Machine Learning, and Kubernetes. Google Cloud provides
services such as Vertex AI and Google Kubernetes Engine (GKE) for AI/ML
workloads and containerized applications.

### 4. What similarities did you observe among the three cloud providers?

The three cloud providers offer similar fundamental infrastructure
capabilities to the resources observed in the KillerCoda Linux environment.
For example, all three provide compute, storage, and networking services,
although the names and specific features of their services are different.

## Sources

- AWS Official Documentation
- Microsoft Azure Official Documentation
- Google Cloud Official Documentation
