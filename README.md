
<div align="center">

</div>

```mermaid
flowchart TB
    A["DEBASISH MOHANTY<br/>INFERENCE PERFORMANCE ENGINEER<br/>Kernel → Serving → Cost"]

    subgraph CORE["CORE ENGINEERING"]
        direction LR
        K["KERNEL ENGINEERING<br/>CUDA C++ · Triton<br/>Shared Memory · Registers<br/>Nsight Compute · Profiling"]
        S["LLM INFERENCE & SERVING<br/>vLLM Source Code<br/>KV-Cache · Continuous Batching<br/>Prefill / Decode · Tensor Parallelism"]
        C["PERFORMANCE & COST<br/>FP8 · GPTQ · AWQ<br/>Roofline Analysis<br/>Accuracy · Cost per Token"]
    end

    G["GPU COMPUTE<br/>CUDA Execution · Memory Hierarchy<br/>T4 · A100 · H100"]

    D["DISTRIBUTED INFERENCE<br/>Multi-GPU Serving · NCCL<br/>Tensor Parallelism · Throughput<br/>Latency · Goodput · SLOs"]

    I["PRODUCTION INFRASTRUCTURE<br/>Kubernetes · AWS · Docker<br/>KEDA · Helm · Terraform<br/>Monitoring · Autoscaling"]

    subgraph PROOF["MEASURED ENGINEERING RESULTS"]
        direction LR
        P1["CUDA ATTENTION<br/>1.81× Speedup<br/>4.655 → 2.566 ms"]
        P2["vLLM SERVING<br/>2.3× Throughput<br/>478 → 1,091 tok/s"]
        P3["QUANTIZATION<br/>37% Lower Cost<br/>Benchmark Result"]
    end

    O["ENGINEERING OUTCOME<br/>↑ Tokens per GPU<br/>↓ Latency<br/>↓ Cost per Token"]

    OSS["OPEN SOURCE<br/>vLLM · Kubernetes Autoscaler<br/>Source-Level Contributions"]

    A --> CORE
    K --> G
    S --> D
    C --> G
    G --> D
    D --> I
    I --> O
    CORE --> PROOF
    PROOF --> O
    A -.-> OSS

    style A fill:#172554,stroke:#60a5fa,color:#ffffff,stroke-width:2px
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
