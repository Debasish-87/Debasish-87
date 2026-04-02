I work on runtime security for Kubernetes — detecting container escapes, privilege escalation, and reverse shells at the syscall layer using eBPF. Most security tools sit too high in the stack. I work closer to the kernel.

---

## Open Source Contributions

| Project | What | Status |
|---|---|---|
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed a file descriptor leak in `libscap` — `taskdir_p` not closed on error paths in `scap_linux_get_threadlist`. Heaptrack: `0B leaked`. | ✅ Merged · v0.24.0 |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Fixed incorrect comments in `registry/client.go` — `ClientOptPlainHTTP`, `LoginOptPlainText`, `Login`. | ✅ Merged |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed broken link to deprecated `kubelet stats v1alpha1` API from node metrics docs. | 🔄 LGTM · on hold |
