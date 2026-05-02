## Open Source Contributions

Contributed to production-grade cloud-native systems by diagnosing and fixing correctness, reliability, and control-plane bugs across Kubernetes and Falco.

## Contributions

| Project | Impact |
|---|---|
| [kubernetes/autoscaler#9506](https://github.com/kubernetes/autoscaler/pull/9506) | Fixed Exoscale node groups ignoring `minSize` (defaulting to 1), causing under-provisioning; restored correct scaling behavior via `NodeGroupSpec` propagation with safe fallback. |
| [kubernetes/autoscaler#9515](https://github.com/kubernetes/autoscaler/pull/9515) | Fixed missing `*/scale` RBAC in VPA Helm chart, restoring admission controller’s ability to resolve CRD selectors. |
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Fixed silent integer overflow (>4GB) in `VMSIZE/VMRSS`, preventing corrupted memory telemetry via `uint64_t` arithmetic. |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in error paths by enforcing deterministic cleanup of `opendir()` handles. |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Corrected registry client documentation to align with actual authentication and HTTP behavior. |
