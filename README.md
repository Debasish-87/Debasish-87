<div align="center">

![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=00F7FF&center=true&vCenter=true&width=600&lines=Kubernetes+Runtime+Security+Engineer;eBPF+%7C+Syscall+Tracing+%7C+Kernel+Security;Falco+%7C+Helm+%7C+Kubernetes+Contributor)

</div>

I build Kubernetes runtime security systems using eBPF — intercepting syscalls to detect and terminate malicious processes in real time. I work at the Linux kernel level, tracing syscalls and translating kernel-level telemetry into deterministic security enforcement.

Active contributor to **Falco**, **Helm**, and **Kubernetes**, with a track record of fixing bugs in production-grade systems.

🔧 **Currently exploring internals of:** `bcc` · `cilium` · `kops`

📬 **Open to full-time roles in:** Runtime Security · eBPF · Kubernetes Infrastructure

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![eBPF](https://img.shields.io/badge/eBPF-000000?style=flat-square&logo=linux&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Falco](https://img.shields.io/badge/Falco-00ADEF?style=flat-square&logo=falco&logoColor=white)
![Cilium](https://img.shields.io/badge/Cilium-F8C517?style=flat-square&logo=cilium&logoColor=black)
![Istio](https://img.shields.io/badge/Istio-466BB0?style=flat-square&logo=istio&logoColor=white)
![Kyverno](https://img.shields.io/badge/Kyverno-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
---

## Open Source Contributions

| Project | Description | Status |
|---|---|---|
| [falcosecurity/libs#2930](https://github.com/falcosecurity/libs/pull/2930) | Fixed integer overflow in thread memory accounting (`VMSIZE`, `VMRSS`) caused by implicit 32-bit arithmetic during KB→byte conversion. Introduced explicit `uint64_t` promotion to ensure correctness for processes >4 GB, preventing corrupted memory telemetry and incorrect security rule evaluation. | ✅ Merged · v0.24.0 |
| [falcosecurity/libs#2926](https://github.com/falcosecurity/libs/pull/2926) | Fixed file descriptor leak in `libscap` (`taskdir_p` not closed on error paths in `scap_linux_get_threadlist`). Verified using Heaptrack — confirmed `0B` memory leaks under test workloads. | ✅ Merged · v0.24.0 |
| [helm/helm#31973](https://github.com/helm/helm/pull/31973) | Corrected misleading documentation in `registry/client.go`, clarifying the behavior of `ClientOptPlainHTTP` and authentication options. | ✅ Merged |
| [kubernetes/website#54593](https://github.com/kubernetes/website/pull/54593) | Removed stale reference to the deprecated `kubelet stats v1alpha1` API from node metrics documentation. | 🔄 LGTM · On Hold |
