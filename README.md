I build Kubernetes runtime security systems using eBPF — intercepting syscalls to detect and terminate malicious processes in real time. I work at the Linux kernel level, tracing syscalls and translating kernel-level telemetry into deterministic security enforcement.

Active contributor to **Falco**, **Helm**, and **Kubernetes**, with a track record of fixing bugs in production-grade systems.

🔧 **Currently exploring internals of:** `bcc` · `cilium` · `kops`

📬 **Open to full-time roles in:** Runtime Security · eBPF · Kubernetes Infrastructure

---

## Open Source Contributions

| Project | Description | Status |
|---|---|---|
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Fixed integer overflow in thread memory accounting (`VMSIZE`, `VMRSS`) caused by implicit 32-bit arithmetic during KB→byte conversion. Introduced explicit `uint64_t` promotion to ensure correctness for processes >4 GB, preventing corrupted memory telemetry and incorrect security rule evaluation. | ✅ Merged · v0.24.0 |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in `libscap` (`taskdir_p` not closed on error paths in `scap_linux_get_threadlist`). Verified using Heaptrack — confirmed `0B` memory leaks under test workloads. | ✅ Merged · v0.24.0 |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Corrected misleading documentation in `registry/client.go`, clarifying the behavior of `ClientOptPlainHTTP` and authentication options. | ✅ Merged |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed stale reference to the deprecated `kubelet stats v1alpha1` API from node metrics documentation. | 🔄 LGTM · On Hold |

---
