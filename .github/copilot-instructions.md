# Kubernetes Vendor Support Matrix

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

This is a documentation-only repository that maintains a Kubernetes version support matrix across different cloud providers and platforms (GKE, AKS, EKS, IKS, OKE, DOKS, OpenShift, RKE, RKE2, TKG, KOPS). The repository contains only Markdown documentation with no code to build, test, or run.

## Working Effectively

### Initial Setup
- Install Node.js and npm for validation tools:
  - `sudo apt update && sudo apt install -y nodejs npm`
- Install markdown validation tools:
  - `npm install markdownlint-cli markdown-link-check`

### Validation Commands (ALWAYS RUN BEFORE COMMITTING)
- Check markdown formatting: `npx markdownlint README.md`
  - Takes <1 second. Expected formatting issues include line length (>80 chars) for table rows.
- Validate external links: `npx markdown-link-check README.md` 
  - Takes ~10-15 seconds. NEVER CANCEL. Some cloud provider links may be temporarily inaccessible.
- Check git status: `git --no-pager status`
- Review changes: `git --no-pager diff`

### Working with the Version Matrix
- The main content is in `README.md` containing a Markdown table of Kubernetes versions vs. vendor support
- Each cell contains either:
  - Specific version numbers (e.g., "1.16.8")
  - Status indicators ("Unsupported", "Deprecated", "preview", "X")
  - "Any*" for RKE indicating flexible version support

### Repository Structure
```
├── README.md           # Main Kubernetes support matrix table
├── LICENSE            # Apache License 2.0
└── .github/
    └── copilot-instructions.md  # This file
```

## Validation Scenarios

### After Making Changes to README.md:
1. **ALWAYS** run markdown linting: `npx markdownlint README.md`
2. **ALWAYS** check external links: `npx markdown-link-check README.md`
3. **ALWAYS** verify table structure is maintained (equal pipe characters across rows)
4. **ALWAYS** ensure vendor reference links in the References section are updated if new vendors are added

### Manual Content Validation:
- Verify all Kubernetes version numbers follow semantic versioning (e.g., 1.16.8)
- Ensure vendor names are consistent: *GKE*, *AKS*, *EKS*, *IKS*, *OKE*, *DOKS*, *OpenShift*, *RKE*, *RKE2*, *TKG*, *KOPS* (italicized)
- Check that "X" is used for future/unavailable versions
- Confirm reference URLs are valid and point to official vendor documentation

## Common Tasks

### Repository Root Contents
```
ls -la
.git
LICENSE
README.md
.gitignore
.github/
```

### Current README.md Structure
- Header: "# Kubernetes Supported Version Matrix"
- Version table with vendors vs Kubernetes versions  
- Note about RKE versioning
- References section with vendor documentation links

### Known Issues
- Some vendor documentation links may be temporarily inaccessible (cloud.google.com, cloud.ibm.com, docs.aws.amazon.com)
- Markdown linting will flag line length violations for table rows (expected behavior)

### Reference Links to Validate
- GKE: https://cloud.google.com/kubernetes-engine/docs/release-notes
- AKS: https://docs.microsoft.com/en-us/azure/aks/supported-kubernetes-versions
- EKS: https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html
- IKS: https://cloud.ibm.com/docs/containers?topic=containers-cs_versions#cs_versions
- OKE: https://docs.oracle.com/en-us/iaas/Content/ContEng/Concepts/contengaboutk8sversions.htm
- DOKS: https://docs.digitalocean.com/products/kubernetes/details/supported-versions/
- OpenShift: https://docs.openshift.com/container-platform/latest/release_notes/ocp-release-notes.html
- RKE: https://github.com/rancher/rke/releases
- RKE2: https://github.com/rancher/rke2/releases
- TKG: https://docs.vmware.com/en/VMware-Tanzu-Kubernetes-Grid/
- KOPS: https://github.com/kubernetes/kops/blob/master/README.md

## Timing Expectations
- Markdown linting: ~2 seconds
- Link checking: ~10-15 seconds (NEVER CANCEL - some external links may be slow)
- Git operations: <1 second each

## Important Notes
- This repository has NO build process, NO test suite, NO application to run
- All work involves updating the Markdown table and documentation
- Focus on maintaining table formatting consistency and accurate version information
- Always validate external reference links after making changes
- Exclude node_modules and package files from git commits (.gitignore handles this)