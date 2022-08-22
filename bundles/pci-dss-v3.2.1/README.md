PREVIEW PCI Data Security Standard v3.2.1
==================================================

## Description

**PREVIEW - Intended for use in test environments only.**

Use the PCI-DSS v3.2.1 policy bundle with [Anthos Policy Controller](https://cloud.google.com/anthos-config-management/docs/concepts/policy-controller) to evaluate the compliance of your in cluster resources against the Payment Card Industry Data Security Standard.

## Compatibility

This bundle requires [Anthos Policy Controller](https://cloud.google.com/anthos-config-management/docs/concepts/policy-controller) v1.12.1+.

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] pci-dss-v3.2.1`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree pci-dss-v3.2.1`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init pci-dss-v3.2.1
kpt fn render pci-dss-v3.2.1
kpt live apply pci-dss-v3.2.1 --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
