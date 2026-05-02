## Open Source Contributions

Contributed to production-grade cloud-native systems by fixing correctness, reliability, and control-plane issues.

## Contributions

| Project | Description |
|---|---|
| [kubernetes/autoscaler#9506](https://github.com/kubernetes/autoscaler/pull/9506) | Fixed Exoscale node groups ignoring configured `minSize`; added proper propagation from `NodeGroupSpec` with safe fallback handling. |
| [kubernetes/autoscaler#9515](https://github.com/kubernetes/autoscaler/pull/9515) | Resolved missing `*/scale` RBAC in VPA admission controller Helm chart, restoring correct CRD selector resolution. |
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Eliminated integer overflow in memory calculations (`VMSIZE/VMRSS`) by promoting arithmetic to `uint64_t`. |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in error path by enforcing proper resource cleanup in `scap_linux_get_threadlist`. |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Corrected misleading registry client documentation to align with actual authentication and HTTP behavior. |
