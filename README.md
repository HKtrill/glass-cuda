# GlassCUDA: Scalable Interpretable Inference Systems Lab

GlassCUDA is an experimental AI systems engineering project focused on accelerating and benchmarking interpretable rule-based inference workloads using CPU and CUDA-based GPU execution.

The project investigates a central systems question:

> Can symbolic and interpretable inference systems scale efficiently under GPU parallelism while preserving transparency and auditability?

GlassCUDA serves as a research-oriented extension of [Project ChurnBot — Interpretable Customer Decision Intelligence](https://github.com/HKtrill/ai-business-coach).

While ChurnBot focused on interpretable predictive modeling, GlassCUDA focuses on the systems engineering and performance characteristics of scalable symbolic inference.

---

# Project Overview

The project combines:

- CUDA programming
- C++ systems engineering
- symbolic rule evaluation
- synthetic workload generation
- CPU/GPU benchmarking
- bitmask-based state encoding
- experiment tracking and analysis
- optional full-stack visualization tooling

---

# Project Goals

GlassCUDA is designed to study how interpretable AI systems behave under large-scale inference workloads.

The project benchmarks:

- CPU vs GPU rule evaluation
- throughput scaling
- memory transfer overhead
- branch divergence
- sparse vs dense symbolic workloads
- batch-size efficiency
- rule evaluations per second
- inference scalability tradeoffs

Rather than focusing on model training, the project focuses specifically on scalable inference execution and benchmarking methodology.

---

# Core Research Question

The project begins with a narrow but important systems question:

> At what workload scale does GPU acceleration become beneficial for symbolic rule-based inference?

GlassCUDA explores situations where:

- CPUs remain more efficient
- GPU overhead dominates runtime
- CUDA acceleration becomes advantageous
- symbolic branching impacts GPU efficiency
- compact state encodings improve scalability

A central design goal is to investigate interpretable AI systems as first-class systems engineering workloads rather than treating explainability as a secondary concern.

---

# Relation to ChurnBot

GlassCUDA complements the earlier ChurnBot research project.

ChurnBot explored:

> Can interpretable AI systems remain competitive with black-box models?

GlassCUDA explores:

> Can interpretable AI systems scale efficiently under high-throughput inference workloads?

Together, the projects support a broader engineering focus on:

> scalable, interpretable, high-performance intelligent systems.

---

# Initial MVP Scope

The initial milestone intentionally remains narrow and measurable:

- CPU rule evaluator
- CUDA rule evaluator
- synthetic workload generator
- benchmark runner
- CSV/JSON benchmark export
- performance plots and technical analysis

Future phases may expand into:

- dashboard visualization
- SQL experiment storage
- Dockerized benchmark environments
- React/TypeScript frontends
- benchmark history analysis
- integration with interpretable rule exports from ChurnBot

---

# Example Workload

GlassCUDA evaluates symbolic rules against feature matrices at scale.

Example:

```text
1,000,000 samples × 10,000 rules × 3 conditions
= 30 billion condition evaluations
```

The project studies how CPU and GPU architectures behave under these workloads and where scalability crossover points emerge.

---

# Example Rule

```text
IF tenure < 6
AND monthly_charges > 90
AND contract_type = month_to_month
THEN predict CHURN
```

The inference engine evaluates:

- which rules fired
- prediction confidence
- abstention states
- runtime performance
- resource allocation
- throughput characteristics

---

# Technical Stack

Planned technologies include:

- C++
- CUDA
- Python
- NumPy / Pandas
- SQLite or PostgreSQL
- React + TypeScript
- Tailwind CSS
- Docker
- GitHub Actions

---

# One-Sentence Summary

> GlassCUDA is a CUDA-accelerated benchmarking platform for scalable interpretable AI inference, designed to study CPU/GPU performance tradeoffs in symbolic rule-based systems.
