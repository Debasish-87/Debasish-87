I build runtime security systems for Kubernetes — using eBPF to intercept syscalls and detect attacks such as reverse shells, privilege escalation, and container escapes in real time.

My work focuses on bridging kernel-level telemetry with deterministic security enforcement in production environments.

Focused on Linux internals, syscall tracing, and container runtime behavior.

I contribute upstream to critical cloud-native infrastructure projects including Falco, Helm, and Kubernetes — fixing bugs in production-grade systems used for runtime security and cluster management.

## Open Source Contributions

| Project | What | Status |
|---|---|---|
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Fixed integer overflow in thread memory accounting (`VMSIZE`, `VMRSS`) caused by implicit 32-bit arithmetic during KB→byte conversion. Introduced explicit `uint64_t` promotion to ensure correctness for processes >4GB, preventing corrupted memory telemetry and incorrect security rule evaluation. | ✅ Merged · v0.24.0 |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in `libscap` (`taskdir_p` not closed on error paths in `scap_linux_get_threadlist`). Verified using Heaptrack — confirmed `0B` memory leaks under test workloads. | ✅ Merged · v0.24.0 |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Corrected misleading documentation in `registry/client.go`, clarifying behavior of `ClientOptPlainHTTP` and authentication options. | ✅ Merged |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed stale reference to deprecated `kubelet stats v1alpha1` API from node metrics documentation. | 🔄 LGTM · on hold |
