# Mike Monaco

**Multi-cloud architect.** 15+ years building production infrastructure — deep AWS roots, with the last two years spent going equally deep on GCP, Azure, and OCI. Everything here is built in public: real, deployable reference architectures, not slideware.

📺 I walk through most of these builds on YouTube: [Mike's Cloud Solutions](https://www.youtube.com/@MikesCloudSolutions)
💼 [LinkedIn](https://www.linkedin.com/in/michael-monaco/) · 📍 North Carolina

---

## The reference architecture matrix

The same core architectures, implemented natively on each major cloud. The design is done once; the provider is an implementation detail.

**Legend:** ✅ built & deployable · 🚧 planned · ✖️ no native equivalent on that provider

### Databases & analytics

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| PostgreSQL | [✅](https://github.com/mamonaco1973/aws-postgres) | [✅](https://github.com/mamonaco1973/gcp-postgres) | [✅](https://github.com/mamonaco1973/azure-postgres) | [✅](https://github.com/mamonaco1973/oci-postgres) |
| MySQL | [✅](https://github.com/mamonaco1973/aws-mysql) | [✅](https://github.com/mamonaco1973/gcp-mysql) | [✅](https://github.com/mamonaco1973/azure-mysql) | [✅](https://github.com/mamonaco1973/oci-mysql) |
| SQL Server | [✅](https://github.com/mamonaco1973/aws-sqlserver) | [✅](https://github.com/mamonaco1973/gcp-sqlserver) | [✅](https://github.com/mamonaco1973/azure-sqlserver) | ✖️ |
| RStudio cluster | [✅](https://github.com/mamonaco1973/aws-rstudio-cluster) | [✅](https://github.com/mamonaco1973/gcp-rstudio-cluster) | [✅](https://github.com/mamonaco1973/azure-rstudio-cluster) | [✅](https://github.com/mamonaco1973/oci-rstudio-cluster) |

### Compute & containers

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Kubernetes | [✅](https://github.com/mamonaco1973/aws-k8s) | [✅](https://github.com/mamonaco1973/gcp-k8s) | [✅](https://github.com/mamonaco1973/azure-k8s) | 🚧 |
| Autoscaling | [✅](https://github.com/mamonaco1973/aws-autoscaling) | [✅](https://github.com/mamonaco1973/gcp-autoscaling) | [✅](https://github.com/mamonaco1973/azure-autoscaling) | [✅](https://github.com/mamonaco1973/oci-autoscaling) |
| Image pipelines (Packer) | [✅](https://github.com/mamonaco1973/aws-packer) | [✅](https://github.com/mamonaco1973/gcp-packer) | [✅](https://github.com/mamonaco1973/azure-packer) | [✅](https://github.com/mamonaco1973/oci-packer) |

### Identity & end-user computing

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Active Directory | [✅](https://github.com/mamonaco1973/aws-active-directory) | [✅](https://github.com/mamonaco1973/gcp-active-directory) | [✅](https://github.com/mamonaco1973/azure-active-directory) | [✅](https://github.com/mamonaco1973/oci-active-directory) |
| Minimal AD (lab-scale) | [✅](https://github.com/mamonaco1973/aws-mini-ad) | [✅](https://github.com/mamonaco1973/gcp-mini-ad) | [✅](https://github.com/mamonaco1973/azure-mini-ad) | [✅](https://github.com/mamonaco1973/oci-mini-ad) |
| Virtual desktops | [✅](https://github.com/mamonaco1973/aws-workspaces) | ✖️ | [✅](https://github.com/mamonaco1973/azure-virtual-desktop) | ✖️ |
| App auth (managed identity / OIDC) | [✅](https://github.com/mamonaco1973/aws-cognito-app) | [✅](https://github.com/mamonaco1973/gcp-cognito-app) | [✅](https://github.com/mamonaco1973/azure-cognito-app) | 🚧 |

### Networking & storage

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Hub-and-spoke networking | [✅](https://github.com/mamonaco1973/aws-transit-gateway) | [✅](https://github.com/mamonaco1973/gcp-transit-gateway) | [✅](https://github.com/mamonaco1973/azure-transit-gateway) | 🚧 |
| Shared file systems | [✅](https://github.com/mamonaco1973/aws-efs) | [✅](https://github.com/mamonaco1973/gcp-efs) | [✅](https://github.com/mamonaco1973/azure-efs) | [✅](https://github.com/mamonaco1973/oci-efs) |
| Data migration | [✅](https://github.com/mamonaco1973/aws-datasync) | 🚧 | 🚧 | 🚧 |

### Serverless

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Serverless CRUD API | [✅](https://github.com/mamonaco1973/aws-serverless-crud) | [✅](https://github.com/mamonaco1973/gcp-serverless-crud) | [✅](https://github.com/mamonaco1973/azure-serverless-crud) | 🚧 |
| Serverless MCP service | [✅](https://github.com/mamonaco1973/aws-serverless-mcp) | [✅](https://github.com/mamonaco1973/gcp-serverless-mcp) | [✅](https://github.com/mamonaco1973/azure-serverless-mcp) | 🚧 |
| Queue-driven workers | [✅](https://github.com/mamonaco1973/aws-sqs-keygen) | [✅](https://github.com/mamonaco1973/gcp-sqs-keygen) | [✅](https://github.com/mamonaco1973/azure-sqs-keygen) | 🚧 |

### AI services

Applications built on each provider's native AI stack — vision, LLM, and agent services, not wrappers around a third-party API.

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Cartoonify (vision AI image transformation) | [✅](https://github.com/mamonaco1973/aws-cartoonify) | [✅](https://github.com/mamonaco1973/gcp-cartoonify) | [✅](https://github.com/mamonaco1973/azure-cartoonify) | 🚧 |
| OpenClaw agent deployment | [✅](https://github.com/mamonaco1973/aws-openclaw) | [✅](https://github.com/mamonaco1973/gcp-openclaw) | [✅](https://github.com/mamonaco1973/azure-openclaw) | 🚧 |
| Resume app (LLM document processing) | [✅](https://github.com/mamonaco1973/aws-resume-app) | [✅](https://github.com/mamonaco1973/gcp-resume-app) | [✅](https://github.com/mamonaco1973/azure-resume-app) | 🚧 |

---

## Builds for fun

Not reference architectures — just things worth building: [aws-xubuntu-xrdp](https://github.com/mamonaco1973/aws-xubuntu-xrdp)

---

## How I work

- **Infrastructure as code, always** — Terraform/HCL first, console only for spelunking
- **Reference architectures over snowflakes** — patterns designed once, ported anywhere
- **AI-accelerated, human-verified** — I use AI tooling to compress build time from weeks to hours; fifteen years of architecture judgment is what makes the output trustworthy

---

*The pinned repos below are the best entry points, or the [YouTube channel](https://www.youtube.com/@MikesCloudSolutions) walks through the major builds end-to-end.*
