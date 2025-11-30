## 🧠 How It Works (v1)

<div align="center">

```mermaid
graph LR
    A[OpenTelemetry Traces] --> B(Causal Graph Builder)
    C[Prometheus Metrics] --> B
    D[CloudWatch Logs] --> E(Log Parser + LLM Embeddings)
    E --> F[Hypothesis Engine]
    B --> F
    F --> G{Risk Assessor}
    G -->|Low Risk| H[Auto-Remediate Tier-3]
    G -->|Medium/High Risk| I[Slack Alert + 1-Click Approve]
    H --> J[Outcome Tracker]
    I --> J
    J --> K[Reinforcement Learning Loop]
