# Orchestration Architecture

```mermaid
flowchart TD
    A[Prompt] --> A1(Primary Orchestrator)
    A1 --> A2(Task Decomposition)
    A2 --> |Single Domain| B[Call Single-Domain Executor]
    A2 --> |Multi-Domain| C[Call Multi-Domain Executor]
'''