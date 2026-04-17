# Open Source Contributions

A collection of merged and in-progress contributions to open source projects across the cloud-native and Kubernetes ecosystem.

## Contributions

| Project | Description | Status |
|---|---|---|
| [kubernetes/autoscaler#9506](https://github.com/kubernetes/autoscaler/pull/9506) | Fixed Exoscale instance pool node groups ignoring configured `minSize` and always defaulting to `1`. Added `minSize`/`maxSize` fields to `instancePoolNodeGroup`, aligned behavior with the SKS nodepool implementation, and introduced a safe fallback with a forward-looking comment for future scale-from-zero support. | ![Merged](https://img.shields.io/badge/MERGED-1a7f37?style=for-the-badge) <br><br> <img src="Screenshots/kubernetes-9506.png" alt="kubernetes-9506 merged" width="350"/> |
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Fixed integer overflow in thread memory accounting (`VMSIZE`, `VMRSS`) caused by implicit 32-bit arithmetic during KB→byte conversion. Introduced explicit `uint64_t` promotion to ensure correctness for processes >4 GB, preventing corrupted memory telemetry and incorrect security rule evaluation. | ![Merged](https://img.shields.io/badge/MERGED-1a7f37?style=for-the-badge) ![v0.24.0](https://img.shields.io/badge/v0.24.0-1a7f37?style=for-the-badge) <br><br> <img src="Screenshots/falcosecurity-2930.png" alt="falcosecurity-2930 merged" width="350"/> |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in `libscap` (`taskdir_p` not closed on error paths in `scap_linux_get_threadlist`). Verified using Heaptrack — confirmed `0B` memory leaks under test workloads. | ![Merged](https://img.shields.io/badge/MERGED-1a7f37?style=for-the-badge) ![v0.24.0](https://img.shields.io/badge/v0.24.0-1a7f37?style=for-the-badge) <br><br> <img src="Screenshots/falcosecurity-2926.png" alt="falcosecurity-2926 merged" width="350"/> |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Corrected misleading documentation in `registry/client.go`, clarifying the behavior of `ClientOptPlainHTTP` and authentication options. | ![Merged](https://img.shields.io/badge/MERGED-1a7f37?style=for-the-badge) |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed stale reference to the deprecated `kubelet stats v1alpha1` API from node metrics documentation. | ![LGTM](https://img.shields.io/badge/LGTM-e8a000?style=for-the-badge) ![On Hold](https://img.shields.io/badge/ON%20HOLD-e8a000?style=for-the-badge) |
