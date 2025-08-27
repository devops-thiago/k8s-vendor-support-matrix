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
| *GKE*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | 1.32.1   | preview  |
| *AKS*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | 1.32.1   | preview  |
| *EKS*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | X        | X        |
| *IKS*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | preview  | X        | X        |
| *OKE*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | 1.32.1   | preview  |
| *DOKS*       | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | 1.32.1   | preview  |
| *OpenShift*  | 4.14+    | 4.15+    | 4.16+    | 4.17+    | 4.18+    | 4.19+    | 4.20+    |
| *RKE*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | X        | X        | X        |
| *RKE2*       | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | 1.32.1   | preview  |
| *TKG*        | 1.27.13  | 1.28.9   | 1.29.4   | 1.30.1   | 1.31.2   | 1.32.1   | preview  |
| *KOPS*       | 1.27.x   | 1.28.x   | 1.29.x   | 1.30.x   | 1.31.x   | X        | X        |

> RKE versions based on the latest release, for older versions you need to use a specific release
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
