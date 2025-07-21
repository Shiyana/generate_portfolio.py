
# AI Data Center Cost Insights

This document provides an overview of capital and operational expenditures for AI data centers, a cost comparison of Cloud vs. On-Prem GPU infrastructure, and strategic recommendations based on real-world examples.

---

## 1. CapEx (Capital Expenditure) Estimates

| Component                               | Estimated Cost        |
|-----------------------------------------|-----------------------|
| Basic Data Center Buildout (per MW)     | 8M - 15M              |
| High-Density GPU Racks (per rack)       | 200K - 400K           |
| Power & Cooling (Liquid/Direct)         | 30–40% of total CapEx |
| Network Infrastructure (Infiniband/10/100GbE) | 1M–3M           |

---

## 2. OpEx (Operational Expenditure)

| Category               | Range / Unit                         |
|------------------------|--------------------------------------|
| Power                  | $0.10–$0.15 per kWh                  |
| Staffing & Ops         | $500K–$1M annually per site          |
| Cooling Maintenance    | $100K–$300K annually                 |
| Hardware Refresh       | Every 3–5 years (~20% annualized)    |
| Support Software Licenses | Varies (open source or vendor support) |

---

## 3. Cloud vs. On-Prem GPU Cost Comparison

| Platform                         | Cost per GPU Hour (USD) |
|---------------------------------|--------------------------|
| AWS / Azure / GCP               | $2.00 – $5.00 (avg ~3.5) |
| Dedicated On-Prem               | $0.80 – $1.50 (avg ~1.15)|
| Shared Community Model (NCShare-like) | $0.60 – $1.00 (avg ~0.8) |

![Cloud vs On-Prem GPU Cost Comparison](cloud_vs_onprem_cost.png)

---

## 4. Recommendations Based on NCShare Goals
- Centralized shared GPU infrastructure at MCNC could reduce costs per institution by **30–50%** vs. cloud.
- Federated Access Model allows small colleges and K–12 to benefit without local infrastructure.
- Utilize **Slurm**, containerized workloads, and LDAP to manage access.
- Backup strategy and redundant LDAP are critical for uptime and multi-user environments.
- Seek grants and vendor credits (AWS, NVIDIA, Dell) to fund initial setup.

---

## 5. Real-World Examples & Use Cases
- **UNC Chapel Hill:** Shared research infrastructure for biomedical and social science applications.
- **Stanford University (HAI):** Uses high-performance GPU clusters (NVIDIA A100s) for AI research.
- **MIT Lincoln Lab:** Operates a Supercloud system combining HPC and AI.
- **Forsyth County Schools (NC):** Leveraged Azure OpenAI to enhance IT support and digital services.

---

## 6. Risks & Sustainability Considerations
- **Energy Costs:** Mitigated with renewable energy credits, peak-shaving strategies, and dynamic cooling.
- **Vendor Lock-In:** Use of container-based workloads and open orchestration prevents dependency.
- **Long-Term Viability:** GPU reuse and power-optimized scheduling help extend infrastructure life.

---

---

## 7. Institutional AI Center Cost Examples

| Institution                                   | Total Investment | Key Features / Takeaway |
|-----------------------------------------------|-----------------|-------------------------|
| **University of Florida – AI Supercomputing Center** | $70M            | HiPerGator AI supercomputer, $25M NVIDIA hardware/software donation. Focus: agriculture, medicine, climate, ethics. Public-private partnership. |
| **MIT Schwarzman College of Computing**       | $1B             | $350M donation from Stephen Schwarzman. Interdisciplinary AI research, ethics, policy, and leadership focus. |
| **San Diego Supercomputer Center (SDSC)**     | $11.5M (Expanse system) | NSF-funded AI/HPC system for AI/ML and biomedical modeling. Federated access model. |
| **MGHPCC (Massachusetts Green HPC Center)**   | $90M            | Shared facility across Harvard, MIT, BU, Northeastern, UMass. Green energy via hydro power. |
| **University of Tennessee + Oak Ridge (Frontier)** | $600M+          | World's fastest supercomputer (as of 2022). National AI and scientific modeling. |

---
