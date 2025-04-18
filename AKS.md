<div align ="center"><h2>Kubernetes Services</h2></div>

<img src="https://github.com/user-attachments/assets/d3e5a542-619e-4831-9209-9fd8fd3cfba4" alt="Alert" width="700"/>

## 1. Deploy application (new)
> Purpose: Deploy your application directly to a Kubernetes cluster.

* This is a wizard-based tool to help you deploy containerized applications quickly to AKS (Azure Kubernetes Service).
* You can specify container images, replica count, ports, and other settings.
* It simplifies the process of writing yaml manifests manually.

## 2. Kubernetes cluster
> Purpose: Create a fully managed AKS cluster.

* This is the option to create an Azure Kubernetes Service (AKS) cluster.
* You get full control over the cluster configuration, including:
    * Node pools
    * Networking
    * Monitoring
    * Authentication
* Best suited for production environments needing scalability and customization.

## 3. Automatic Kubernetes cluster (preview)
> Purpose: Quickly deploy a Kubernetes cluster with automated settings (currently in preview).

* Automatically provisions the AKS cluster using best practice defaults.
* Minimizes setup time for developers who want to focus on deploying apps rather than managing infrastructure.
* May include built-in GitOps, monitoring, etc.
* Preview means it's in a testing phase and may change.

## 4. Add a Kubernetes cluster with Azure Arc
> Purpose: Connect an existing on-premises or multi-cloud Kubernetes cluster to Azure.

* Azure Arc lets you manage non-Azure Kubernetes clusters from within Azure.
* Useful for hybrid or multi-cloud scenarios.
* Provides visibility and governance using Azure tools (like Policy, Monitor, etc.)

## 5. Create a Kubernetes cluster with Azure Arc
> Purpose: Use Azure Arc to provision a Kubernetes cluster outside of Azure (e.g., on your VM or bare metal).

* You can create and onboard a new Kubernetes cluster that’s not in Azure but still manageable from Azure.
* Useful for organizations with existing infrastructure outside Azure wanting centralized control.

