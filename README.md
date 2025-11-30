# Autonoma

> **Augmented Autonomy for Cloud-Native Operations**  
> Reduce MTTR by 50%+ with AI-assisted root cause analysis and safe, human-approved remediation.

Autonoma is **not** an "autonomous AI." It’s a **reinforcement learning system** that:
- Diagnoses incidents using causal inference over OpenTelemetry traces + metrics
- Proposes remediations with **validated safety gates**
- Learns from every action/outcome to prevent recurrence  
- **Never acts autonomously on Tier-1 services** without human approval

Built for SREs who want **confidence, not magic**.

---

## 🔑 Core Principles

1. **Safety First**: All actions pass risk validation (blast radius, success history, business impact).
2. **Explainability**: Every diagnosis includes evidence chain (logs, traces, metrics).
3. **Incremental Autonomy**: Starts as a copilot → evolves to auto-remediate only after proven reliability.
4. **Single-Cloud Focused**: v1 supports **AWS EKS + EC2**. Multi-cloud is a future concern.

---

## 🚀 Quick Start (Local Dev)

```bash
# Requires: Docker, k3d, Python 3.10+
git clone https://github.com/yourorg/autonoma-core.git
cd autonoma-core
make dev-env       # Spins up k3d cluster + demo app
make run           # Starts Autonoma agent
