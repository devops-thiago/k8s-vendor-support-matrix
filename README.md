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
| *GKE*        | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | 1.33.1   |
| *AKS*        | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | 1.33.1   |
| *EKS*        | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | preview  |
| *IKS*        | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | preview  | preview  |
| *OKE*        | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | preview  |
| *DOKS*       | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | 1.33.1   |
| *OpenShift*  | Unsupported | Unsupported | 4.16+    | 4.17+    | 4.18+    | 4.19+    | 4.20+    |
| *RKE*        | 1.27.16  | 1.28.15  | 1.29.9   | 1.30.6   | X        | X        | X        |
| *RKE2*       | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | preview  |
| *TKG*        | Deprecated | Deprecated | 1.29.9   | 1.30.6   | 1.31.3   | 1.32.2   | preview  |
| *KOPS*       | Deprecated | Deprecated | 1.29.x   | 1.30.x   | 1.31.x   | 1.32.x   | preview  |

> RKE versions based on the latest release, for older versions you need to use a specific release

> **Status Indicators:**
> - **Specific version** (e.g., 1.30.6): Fully supported and available for deployment
> - **preview**: Available in preview/beta, not yet generally available
> - **Deprecated**: Still available but deprecated, will be removed in future releases
> - **Unsupported**: No longer available for new deployments
> - **X**: Not supported or not yet available

> **Note:** The version numbers shown for OpenShift (e.g., 4.10+, 4.11+, etc.) are OpenShift platform versions, *not* Kubernetes versions. This differs from all other vendors in the table, who show Kubernetes versions. OpenShift versions follow Red Hat's versioning scheme and may include custom Kubernetes patches.

## References
*GKE* - [https://cloud.google.com/kubernetes-engine/docs/release-notes](https://cloud.google.com/kubernetes-engine/docs/release-notes)

*AKS* - [https://docs.microsoft.com/en-us/azure/aks/supported-kubernetes-versions](https://docs.microsoft.com/en-us/azure/aks/supported-kubernetes-versions)

*EKS* - [https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html)

*IKS* - [https://cloud.ibm.com/docs/containers?topic=containers-cs_versions#cs_versions](https://cloud.ibm.com/docs/containers?topic=containers-cs_versions#cs_versions)

*OKE* - [https://docs.oracle.com/en-us/iaas/Content/ContEng/Concepts/contengaboutk8sversions.htm](https://docs.oracle.com/en-us/iaas/Content/ContEng/Concepts/contengaboutk8sversions.htm)

*DOKS* - [https://docs.digitalocean.com/products/kubernetes/details/supported-versions/](https://docs.digitalocean.com/products/kubernetes/details/supported-versions/)

*OpenShift* - [https://docs.openshift.com/container-platform/latest/release_notes/ocp-release-notes.html](https://docs.openshift.com/container-platform/latest/release_notes/ocp-release-notes.html)

*RKE* - [https://github.com/rancher/rke/releases](https://github.com/rancher/rke/releases)

*RKE2* - [https://github.com/rancher/rke2/releases](https://github.com/rancher/rke2/releases)

*TKG* - [https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/](https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/)

*KOPS* - [https://github.com/kubernetes/kops/releases](https://github.com/kubernetes/kops/releases)
