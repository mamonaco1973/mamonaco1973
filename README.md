# Mike Monaco

**Multi-cloud architect.** 15+ years building production infrastructure — deep AWS roots, with the last two years spent going equally deep on GCP, Azure, and OCI. Everything here is built in public: real, deployable reference architectures, not slideware.

📺 I walk through most of these builds on YouTube: [Mike's Cloud Solutions](https://www.youtube.com/@MikesCloudSolutions)
💼 [LinkedIn](https://www.linkedin.com/in/michael-monaco/) · 📍 North Carolina

---

## What this portfolio demonstrates

The same core architectures — networking, identity, compute, Kubernetes, databases, serverless — implemented natively on each major cloud provider. The goal: prove that good architecture is portable, and that the provider is an implementation detail.

A recent example: I ported my AWS PostgreSQL/MySQL reference architecture to OCI in an afternoon, because the design work was already done. That's the thesis of this repo collection.

---

## Reference architectures by provider

### ☁️ AWS
| Repo | What it shows |
|---|---|
| [aws-serverless-mcp](https://github.com/mamonaco1973/aws-serverless-mcp) | Serverless MCP service — Lambda, API Gateway, IaC in Terraform |
| [aws-packer](https://github.com/mamonaco1973/aws-packer) | Golden AMI pipeline with Packer |
| [aws-ssm](https://github.com/mamonaco1973/aws-ssm) | Systems Manager patterns for fleet management |
| <!-- ADD: your best AWS database reference architecture repo --> | RDS PostgreSQL/MySQL reference architecture |

### ☁️ Google Cloud
| Repo | What it shows |
|---|---|
| [gcp-k8s](https://github.com/mamonaco1973/gcp-k8s) | GKE Kubernetes reference deployment |
| [gcp-openclaw](https://github.com/mamonaco1973/gcp-openclaw) | <!-- one line on what this demonstrates --> |
| <!-- ADD: 1-2 more of your strongest GCP repos --> | |

### ☁️ Azure
| Repo | What it shows |
|---|---|
| <!-- ADD: your strongest Azure repos --> | |

### ☁️ Oracle Cloud (OCI)
| Repo | What it shows |
|---|---|
| <!-- ADD: the OCI database port and other OCI repos --> | PostgreSQL/MySQL reference architecture ported from AWS |


---

## How I work

- **Infrastructure as code, always** — Terraform/HCL first, console only for spelunking
- **Reference architectures over snowflakes** — patterns designed once, ported anywhere
- **AI-accelerated, human-verified** — I use AI tooling to compress build time from weeks to hours; fifteen years of architecture judgment is what makes the output trustworthy

---

*Looking at the repo list and not sure where to start? The pinned repos below are the best entry points, or the [YouTube channel](https://www.youtube.com/@MikesCloudSolutions) walks through the major builds end-to-end.*
