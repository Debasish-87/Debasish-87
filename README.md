<div align="center">

```text
┌──────────────────────────────────────────────────────────────────────────────┐
│                    PERFORMANCE ENGINEER, GPU & INFERENCE                     │
│                          Kernel → Serving → Cost                             │
├──────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  ┌────────────────────┐  ┌────────────────────┐  ┌────────────────────┐      │
│  │ KERNEL ENGINEERING │  │  LLM INFERENCE     │  │ PERFORMANCE & COST │      │
│  ├────────────────────┤  ├────────────────────┤  ├────────────────────┤      │
│  │ CUDA C++           │  │ vLLM Source Code   │  │ FP8 / GPTQ / AWQ   │      │
│  │ Triton             │  │ KV-Cache           │  │ Roofline Analysis  │      │
│  │ Shared Memory      │  │ Continuous Batching│  │ Accuracy           │      │
│  │ Register Tuning    │  │ Prefill / Decode   │  │ Cost per Token     │      │
│  │ Nsight Compute     │  │ Tensor Parallelism │  │ Latency / Goodput  │      │
│  └──────────┬─────────┘  └──────────┬─────────┘  └──────────┬─────────┘      │
│             │                       │                       │                │
│             └───────────────────────┼───────────────────────┘                │
│                                     ▼                                        │
│                   ┌──────────────────────────────────┐                       │
│                   │           GPU COMPUTE            │                       │
│                   │ CUDA Execution · Memory Hierarchy│                       │
│                   │       NVIDIA T4 / A100 / H100    │                       │
│                   └───────────────┬──────────────────┘                       │
│                                   ▼                                          │
│                   ┌───────────────────────────────────┐                      │
│                   │       DISTRIBUTED INFERENCE       │                      │
│                   │ Multi-GPU · NCCL · Tensor Parallel│                      │
│                   │ Throughput · Latency · Goodput    │                      │
│                   └───────────────┬───────────────────┘                      │
│                                   ▼                                          │
│                   ┌─────────────────────────────────┐                        │
│                   │    PRODUCTION INFRASTRUCTURE    │                        │
│                   │ Kubernetes · AWS · Docker       │                        │
│                   │ KEDA · Helm · Terraform         │                        │
│                   │ Monitoring · Autoscaling        │                        │
│                   └───────────────┬─────────────────┘                        │
│                                   ▼                                          │
├──────────────────────────────────────────────────────────────────────────────┤
│                         ENGINEERING OUTCOMES                                 │
│      ↑ GPU Throughput  ·  ↓ Inference Latency  ·  ↓ Cost per Token           │
└──────────────────────────────────────────────────────────────────────────────┘
```

![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Triton](https://img.shields.io/badge/Triton-6A5ACD?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-000000?style=flat-square)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

`CUDA/GPU → vLLM → Distributed Inference → Kubernetes → AWS`

contributor to [vLLM](https://github.com/vllm-project/vllm) and [Kubernetes](https://github.com/kubernetes/autoscaler)

</div>
