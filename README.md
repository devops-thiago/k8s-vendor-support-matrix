# Kubernetes Supported Version Matrix

## Vendors

- **GKE**: Google Kubernetes Engine
- **AKS**: Azure Kubernetes Service
- **EKS**: Amazon Elastic Kubernetes Service
- **IKS**: IBM Kubernetes Service
- **OKE**: Oracle Container Engine for Kubernetes
- **DOKS**: DigitalOcean Kubernetes
- **OpenShift**: Red Hat OpenShift Container Platform
- **RKE**: Rancher Kubernetes Engine
- **RKE2**: Rancher Kubernetes Engine v2
- **TKG**: VMware Tanzu Kubernetes Grid
- **KOPS**: Kubernetes Operations

| *Kubernetes* | *1.27.x* | *1.28.x* | *1.29.x* | *1.30.x* | *1.31.x* | *1.32.x* | *1.33.x* |
|--------------|----------|----------|----------|----------|----------|----------|----------|
| *GKE*        | End-of-Life | Extended Support | 1.29.15  | 1.30.14  | 1.31.12  | 1.32.8   | 1.33.4   |
| *AKS*        | End-of-Life | Extended Support | 1.29.15  | 1.30.14  | 1.31.12  | 1.32.8   | 1.33.4   |
| *EKS*        | End-of-Life | Extended Support | 1.29.15  | 1.30.14  | 1.31.12  | 1.32.8   | 1.33.4   |
| *IKS*        | End-of-Life | Extended Support | 1.29.15  | 1.30.14     | 1.31.12  | 1.32.8   | preview  |
| *OKE*        | End-of-Life | Extended Support | 1.29.15  | 1.30.14  | 1.31.12  | 1.32.8   | preview  |
| *DOKS*       | End-of-Life | Extended Support | 1.29.15  | 1.30.14  | 1.31.12  | 1.32.8   | 1.33.4   |
| *OpenShift*  | Unsupported | End-of-Life | 4.16+    | 4.17+    | 4.18+    | 4.19+    | 4.20+    |
| *RKE*        | 1.27.16  | 1.28.15  | 1.29.15  | 1.30.14  | 1.31.11  | 1.32.7   | X        |
| *RKE2*       | End-of-Life | Extended Support | 1.29.15  | 1.30.14     | 1.31.12  | 1.32.8   | 1.33.4   |
| *TKG*        | End-of-Life | Extended Support | 1.29.15  | 1.30.14  | 1.31.12  | 1.32.8   | preview  |
| *KOPS*       | End-of-Life | Extended Support | 1.29.x   | 1.30.x   | 1.31.x   | 1.32.x   | preview  |

> RKE versions based on the latest release, for older versions you need to use a specific release

> **Status Indicators:**
>
> - **Specific version** (e.g., 1.30.6): Fully supported and available for new deployments
> - **LTS**: Long-term support version with extended maintenance lifecycle
> - **Extended Support**: Still supported but with limited updates, maintenance mode only
> - **End-of-Life**: No longer supported, security updates may be unavailable
> - **Unsupported**: Never supported or completely discontinued
> - **preview**: Available in preview/beta, not yet generally available
> - **X**: Not supported or not yet available

> **Note:** The version numbers shown for OpenShift (e.g., 4.10+, 4.11+, etc.) are OpenShift platform versions, *not* Kubernetes versions. This differs from all other vendors in the table, who show Kubernetes versions. OpenShift versions follow Red Hat's versioning scheme and may include custom Kubernetes patches.

## Vendor Support Policy Details

Different vendors have varying support policies for Kubernetes versions:

### Cloud Providers (GKE, AKS, EKS, IKS, OKE)

- **End-of-Life**: Kubernetes versions are automatically deprecated and eventually removed from new cluster creation
- **Extended Support**: Some providers offer extended support for older versions (typically for enterprise customers)
- **LTS**: Long-term support versions are maintained for extended periods with security updates

### DigitalOcean Kubernetes (DOKS)

- Uses a more aggressive deprecation policy with shorter support windows
- Focuses on recent stable versions for optimal performance and security

### Red Hat OpenShift

- Follows Red Hat's enterprise support lifecycle
- **Unsupported**: Very old versions are completely discontinued
- **End-of-Life**: Versions no longer receiving updates but may still be deployable

### Rancher (RKE/RKE2)

- RKE maintains broader version support across the Kubernetes release spectrum
- RKE2 follows a more structured support model with clear LTS designations

### VMware TKG & KOPS

- Follow upstream Kubernetes support policies closely
- Provide extended support for enterprise deployments

## References

*GKE* - [https://cloud.google.com/kubernetes-engine/docs/release-notes](https://cloud.google.com/kubernetes-engine/docs/release-notes)

*AKS* - [https://docs.microsoft.com/en-us/azure/aks/supported-kubernetes-versions](https://docs.microsoft.com/en-us/azure/aks/supported-kubernetes-versions)

*EKS* - [https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html)

*IKS* - [https://cloud.ibm.com/docs/containers?topic=containers-cs_versions#cs_versions](https://cloud.ibm.com/docs/containers?topic=containers-cs_versions#cs_versions)

*OKE* - [https://docs.oracle.com/en-us/iaas/Content/ContEng/Concepts/contengaboutk8sversions.htm](https://docs.oracle.com/en-us/iaas/Content/ContEng/Concepts/contengaboutk8sversions.htm)

*DOKS* - [https://docs.digitalocean.com/products/kubernetes/](https://docs.digitalocean.com/products/kubernetes/)

*OpenShift* - [https://docs.openshift.com/container-platform/latest/release_notes/ocp-release-notes.html](https://docs.openshift.com/container-platform/latest/release_notes/ocp-release-notes.html)

*RKE* - [https://github.com/rancher/rke/releases](https://github.com/rancher/rke/releases)

*RKE2* - [https://github.com/rancher/rke2/releases](https://github.com/rancher/rke2/releases)

*TKG* - [https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/)

*KOPS* - [https://github.com/kubernetes/kops/releases](https://github.com/kubernetes/kops/releases)
