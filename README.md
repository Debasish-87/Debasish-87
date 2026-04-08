I build security tooling for Kubernetes — intercepting syscalls via eBPF to detect and stop attacks at runtime, enforcing secure configurations pre-deployment, and enabling safe progressive rollouts with Istio traffic splitting.

I also contribute upstream to the systems I rely on — Falco, Helm, and Kubernetes — fixing real bugs in production-grade codebases.

## Open Source Contributions

| Project | What | Status |
|---|---|---|
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Fixed integer overflow in thread memory accounting (`VMSIZE`, `VMRSS`) caused by implicit 32-bit arithmetic during KB→byte conversion. Applied safe `uint64_t` promotion to ensure correct telemetry for processes >4GB and prevent rule mis-evaluation in runtime detection. | ✅ Merged · v0.24.0 |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in `libscap` — `taskdir_p` not closed on error paths in `scap_linux_get_threadlist`. Verified via Heaptrack (`0B leaked`). | ✅ Merged · v0.24.0 |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Fixed incorrect documentation/comments in `registry/client.go` affecting `ClientOptPlainHTTP` and login options. | ✅ Merged |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed broken reference to deprecated `kubelet stats v1alpha1` API from node metrics docs. | 🔄 LGTM · on hold |
