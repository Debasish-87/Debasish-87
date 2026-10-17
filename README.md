
<div align="center">

</div>

```mermaid
flowchart LR
    A["DEBASISH MOHANTY<br/>INFERENCE PERFORMANCE ENGINEER<br/>Kernel → Serving → Cost"]

    subgraph CORE["CORE ENGINEERING"]
        direction LR
        K["KERNEL ENGINEERING<br/>CUDA C++ | Triton<br/>Shared Memory | Registers<br/>Nsight Compute | Profiling"]
        S["LLM INFERENCE & SERVING<br/>vLLM | KV-Cache<br/>Continuous Batching<br/>Prefill / Decode | Tensor Parallelism"]
        C["PERFORMANCE & COST OPTIMIZATION<br/>FP8 | GPTQ | AWQ<br/>Roofline Analysis<br/>Latency | Throughput | Cost per Token"]
    end

    subgraph COMPUTE["GPU COMPUTE & DISTRIBUTED INFERENCE"]
        direction LR
        G["GPU ARCHITECTURE<br/>CUDA Execution | Memory Hierarchy<br/>T4 | A100 | H100"]
        D["DISTRIBUTED INFERENCE<br/>NCCL | Multi-GPU Serving<br/>Throughput | Latency | Goodput | SLOs"]
    end

    I["PRODUCTION INFRASTRUCTURE<br/>Kubernetes | AWS | Docker<br/>KEDA | Helm | Terraform<br/>Monitoring | Autoscaling"]

    subgraph RESULTS["MEASURED ENGINEERING RESULTS"]
        direction LR
        P1["CUDA ATTENTION KERNEL<br/>1.81x Speedup<br/>4.655 ms → 2.566 ms"]
        P2["vLLM INFERENCE SERVING<br/>2.3x Throughput<br/>478 → 1,091 tokens/sec"]
        P3["MODEL QUANTIZATION<br/>37% Lower Cost per Token<br/>Benchmark Result"]
    end

    O["PERFORMANCE OUTCOMES<br/>Higher GPU Throughput<br/>Lower Inference Latency<br/>Lower Cost per Token"]

    OSS["OPEN SOURCE CONTRIBUTIONS<br/>vLLM | Kubernetes Autoscaler"]

    A --> CORE
    K --> G
    S --> D
    C --> G
    G --> D
    D --> I
    CORE --> RESULTS
    I --> O
    RESULTS --> O
    O -.-> OSS

    style A fill:#172554,stroke:#60a5fa,color:#ffffff,stroke-width:3px
    style K fill:#111827,stroke:#60a5fa,color:#ffffff
    style S fill:#111827,stroke:#60a5fa,color:#ffffff
    style C fill:#111827,stroke:#60a5fa,color:#ffffff
    style G fill:#172554,stroke:#818cf8,color:#ffffff
    style D fill:#172554,stroke:#818cf8,color:#ffffff
    style I fill:#1e293b,stroke:#94a3b8,color:#ffffff
    style P1 fill:#052e16,stroke:#4ade80,color:#ffffff
    style P2 fill:#052e16,stroke:#4ade80,color:#ffffff
    style P3 fill:#052e16,stroke:#4ade80,color:#ffffff
    style O fill:#14532d,stroke:#4ade80,color:#ffffff,stroke-width:2px
    style OSS fill:#312e81,stroke:#a5b4fc,color:#ffffff
```

<div align="center">

**CUDA · C++ · Python · Triton · PyTorch · vLLM · NCCL · Kubernetes · AWS · Terraform**

</div>
