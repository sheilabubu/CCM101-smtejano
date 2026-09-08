# Cloud Platform Recommendations

## Client A – Startup Company

### Recommended Cloud Platform: Google Cloud Platform (GCP)

Google Cloud is a good option for the startup because it provides scalable cloud resources that can grow together with the company. Also a startup can begin with basic services and expand the infrastructure as the number of customers increases. Google Cloud also provides managed services that can reduce the need for a small development team to handle complex infrastructure tasks, it is pay-as-you-use approach can also help the company avoid investing heavily in physical hardware.

### Recommended Services

* **Compute Engine** – for hosting backend servers and application workloads.
* **Cloud Storage** – for storing application files, images, and backups.
* **Cloud SQL** – for managing the application's relational database.
* **Cloud Load Balancing** – for distributing application traffic and improving availability.

---

## Client B – University

### Recommended Cloud Platform: Microsoft Azure

Microsoft Azure is a suitable choice for the university because it can work closely with the university's existing Microsoft environment. Since the institution already uses Windows Server, Microsoft 365, and Active Directory, moving workloads to Azure can provide better compatibility and easier centralized management. Azure can also support student systems, administrative applications, databases, and other university services.

### Recommended Services

* **Azure Virtual Machines** – for running existing Windows Server applications.
* **Microsoft Entra ID** – for managing student, faculty, and staff identities and access.
* **Azure Virtual Network** – for connecting and isolating university cloud resources.
* **Azure SQL Database** – for storing and managing university application data.

---

## Client C – AI Research Company

### Recommended Cloud Platform: Google Cloud Platform (GCP)

Google Cloud is highly suitable for the AI research company because of strong focus on artificial intelligence, machine learning, and data processing. The company can use Google Cloud's computing infrastructure and specialized hardware to perform demanding AI experiments, it can also use managed AI services to develop and deploy machine learning models without building the entire infrastructure from the beginning.

### Recommended Services

* **Vertex AI** – for building, training, testing, and deploying machine learning models.
* **Compute Engine** – for running customized high-performance computing workloads.
* **Google Kubernetes Engine (GKE)** – for deploying scalable containerized AI applications.
* **Cloud Storage** – for storing training datasets, research files, and AI models.

---

## Client D – Global E-Commerce Company

### Recommended Cloud Platform: Microsoft Azure

Microsoft Azure can be a strong choice for the global e-commerce company because it provides scalable computing, networking, database, and content delivery services. The company can distribute applications across different Azure regions to serve international customers. Azure's scaling and load-balancing capabilities can also help the company handle sudden increases in website traffic during promotions and peak shopping seasons.

### Recommended Services

* **Azure Virtual Machines** – for hosting web servers and application workloads.
* **Azure Load Balancer** – for distributing network traffic across available resources.
* **Virtual Machine Scale Sets** – for automatically increasing or decreasing virtual machine capacity.
* **Azure SQL Database** – for managing customer, product, and transaction data.
* **Azure Front Door** – for improving global application delivery and routing users to suitable endpoints.

# Multi-Cloud Decision Matrix

| Business Requirement               | Recommended Platform | Justification                                                                                                                                                          |
| ---------------------------------- | -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Startup Business                   | AWS                  | AWS provides flexible cloud services that allow a startup to begin with basic resources and expand its infrastructure as the business grows.                           |
| Large Enterprise                   | Azure                | Azure offers strong enterprise management, security, identity services, and integration with business technologies, making it suitable for large organizations.        |
| Microsoft-Based Environment        | Azure                | Azure is closely connected with Microsoft products such as Windows Server, Microsoft 365, and Microsoft Entra ID, providing easier integration and management.         |
| Artificial Intelligence / ML       | GCP                  | Google Cloud provides specialized AI and machine learning services, including Vertex AI, as well as computing resources designed for demanding AI workloads.           |
| Container and Kubernetes Workloads | GCP                  | Google Kubernetes Engine (GKE) provides managed Kubernetes capabilities that simplify the deployment, scaling, and management of containerized applications.           |
| International Web Application      | AWS                  | AWS offers a large global infrastructure, scalable computing, load balancing, and content delivery services that can support applications with users around the world. |

## Sources
https://docs.aws.amazon.com/

https://learn.microsoft.com/en-us/azure/?product=popular

https://docs.cloud.google.com/
