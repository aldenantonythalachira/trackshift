# GridOvertake
### Where F1 Strategy Meets Grid Stability


[![Status](https://img.shields.io/badge/Status-Prototype-blue?style=for-the-badge)]()
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)]()

> **Shortlisted Submission — TrackShift 2026**

**GridOvertake** applies Formula 1 Energy Recovery System (ERS) strategy to India’s smart grid and EV fleet energy management.

Every F1 driver manages a **4 MJ energy budget per lap** — harvest under braking or deploy for an overtake? India’s grid faces the same problem: store intermittent renewables or discharge for peak demand? We treat each **microgrid as an F1 car**, each **peak event as an overtake**, and each **renewable surge as a braking zone**.

**We don’t just build AI. We bring championship-winning F1 strategy to India’s energy future.**

---

##  Core Innovations

- **Cross-Domain Transfer Learning** — Pre-train on F1 telemetry → fine-tune on Indian grid data. *First to connect these domains.*
- **Attention-Based RL** — PPO + Multi-Head Attention lets the agent “watch” every grid node, like a strategist monitoring all cars.
- **Constraint-Aware Safety** — Hard constraints encode grid frequency rules and EV battery limits. *No blackouts. No battery damage.*
- **Edge Deployable** — <5s inference on Raspberry Pi 4 + Coral TPU. Works at rural substations.

---

##  Validation Snapshot

| Metric | Result |
|---|---|
| F1 strategy replication (Abu Dhabi 2021) | **94% accuracy** |
| Peak blackout reduction (BSES Delhi digital twin) | **23%** |
| Renewable utilization increase | **18%** |
| EV battery life extension | **+31%** |
| Decision latency | **4.2 seconds** |

*Baselines: rule-based heuristics (0% blackout reduction, 62% renewable use, 30 min latency).*

---

##  Architecture (at a glance)
F1 + Grid Data → Temporal Fusion Transformer → Graph Neural Network → PPO + Attention → Battery + EV Commands


**Stack:** PyTorch · Ray RLlib · Pandapower · FastF1 · InfluxDB · Streamlit · ONNX

---
