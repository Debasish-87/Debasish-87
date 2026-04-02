I build security tooling for Kubernetes — intercepting syscalls via eBPF to catch attacks at runtime, blocking insecure configs before they reach production, and managing safe rollouts with Istio traffic splitting. I also contribute to the upstream projects I depend on — Falco, Helm, and Kubernetes.

## Open Source Contributions

| Project | What | Status |
|---|---|---|
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed a file descriptor leak in `libscap` — `taskdir_p` not closed on error paths in `scap_linux_get_threadlist`. Heaptrack: `0B leaked`. | ✅ Merged · v0.24.0 |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Fixed incorrect comments in `registry/client.go` — `ClientOptPlainHTTP`, `LoginOptPlainText`, `Login`. | ✅ Merged |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed broken link to deprecated `kubelet stats v1alpha1` API from node metrics docs. | 🔄 LGTM · on hold |
