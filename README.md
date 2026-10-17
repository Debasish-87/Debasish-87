
<div align="center">

# Debasish Mohanty

### Inference Performance Engineer

**Optimizing LLM inference for throughput, latency, and cost.**

`Kernel → Serving → Cost`

</div>

---

## <div align="center">INFERENCE PERFORMANCE ARCHITECTURE</div>

```mermaid
flowchart TB
    A["INFERENCE PERFORMANCE ENGINEER"]

    subgraph WORK["CORE ENGINEERING"]
        direction LR
        K["KERNEL<br/>CUDA C++ · Triton<br/>Nsight · Shared Memory"]
        S["SERVING<br/>vLLM · KV-Cache<br/>Batching · Tensor Parallelism"]
        C["COST<br/>FP8 · GPTQ / AWQ<br/>Roofline · Cost per Token"]
    end

    G["GPU COMPUTE<br/>T4 · A100 · H100"]
    I["INFRASTRUCTURE<br/>Kubernetes · AWS · Docker"]
    O["OUTCOME<br/>↑ Throughput · ↓ Latency · ↓ Cost"]

    A --> WORK
    K --> G
    S --> G
    C --> G
    G --> I
    I --> O

    style A fill:#172554,stroke:#60a5fa,color:#ffffff
    style K fill:#111827,stroke:#60a5fa,color:#ffffff
    style S fill:#111827,stroke:#60a5fa,color:#ffffff
    style C fill:#111827,stroke:#60a5fa,color:#ffffff
    style G fill:#172554,stroke:#60a5fa,color:#ffffff
    style I fill:#172554,stroke:#60a5fa,color:#ffffff
    style O fill:#14532d,stroke:#4ade80,color:#ffffff
```

---

## <div align="center">SELECTED BENCHMARKS</div>

<div align="center">

| Project | Measured Result |
|:---|:---:|
| CUDA Attention Kernel | **1.81× speedup** |
| Multi-GPU vLLM Serving | **2.3× throughput** |
| Quantization Benchmark | **37% lower cost/token** |

</div>

---

## <div align="center">PINNED PROJECTS</div>

<div align="center">

**[Inference Performance](https://github.com/Debasish-87/inference-performance)** · **[GPU Attention](https://github.com/Debasish-87/gpu-attention-performance)**

**[Quantization Benchmark](https://github.com/Debasish-87/quantization-benchmark)** · **[vLLM Inference Operator](https://github.com/Debasish-87/vllm-inference-operator)**

</div>

---

<div align="center">

**CUDA/GPU → vLLM → Distributed Inference → Kubernetes → AWS**

[GitHub](https://github.com/Debasish-87) · [Website](https://www.debasishmohanty.in/) · [LinkedIn](https://www.linkedin.com/in/debasishmohanty87/)

</div>
