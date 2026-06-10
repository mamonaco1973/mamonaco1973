# Mike Monaco

**Multi-cloud architect.** 10+ years building production infrastructure — deep AWS roots, with the last two years spent going equally deep on GCP, Azure, and OCI. Everything here is built in public: real, deployable reference architectures, not slideware.

> **[Ask Mike](https://askmike.mikes-cloud-solutions.com)** — AI assistant trained on Mike's background, projects, and cloud portfolio. Ask about any architecture, compare patterns across providers, or ask interview questions.

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
| RStudio on Kubernetes | [✅](https://github.com/mamonaco1973/aws-rstudio-eks) | [✅](https://github.com/mamonaco1973/gcp-rstudio-gke) | [✅](https://github.com/mamonaco1973/azure-rstudio-aks) | 🚧 |

### Compute & containers

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Kubernetes | [✅](https://github.com/mamonaco1973/aws-k8s) | [✅](https://github.com/mamonaco1973/gcp-k8s) | [✅](https://github.com/mamonaco1973/azure-k8s) | 🚧 |
| Autoscaling (ASG / MIG / VMSS / instance pools) | [✅](https://github.com/mamonaco1973/aws-autoscaling) | [✅](https://github.com/mamonaco1973/gcp-mig) | [✅](https://github.com/mamonaco1973/azure-vmss) | [✅](https://github.com/mamonaco1973/oci-instance-pool) |
| Autoscaled Flask application | [✅](https://github.com/mamonaco1973/aws-flask-asg) | [✅](https://github.com/mamonaco1973/gcp-flask-mig) | [✅](https://github.com/mamonaco1973/azure-flask-vmss) | 🚧 |
| Containerized Flask application | [✅](https://github.com/mamonaco1973/aws-flask-container) | [✅](https://github.com/mamonaco1973/gcp-flask-container) | [✅](https://github.com/mamonaco1973/azure-flask-container) | 🚧 |
| Image pipelines (Packer) | [✅](https://github.com/mamonaco1973/aws-packer) | [✅](https://github.com/mamonaco1973/gcp-packer) | [✅](https://github.com/mamonaco1973/azure-packer) | [✅](https://github.com/mamonaco1973/oci-packer) |

### Identity & end-user computing

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Managed directory services | [✅](https://github.com/mamonaco1973/aws-active-directory) | [✅](https://github.com/mamonaco1973/gcp-directory) | [✅](https://github.com/mamonaco1973/azure-directory) | [✅](https://github.com/mamonaco1973/oci-managed-ad) |
| Minimal AD (lab-scale) | [✅](https://github.com/mamonaco1973/aws-mini-ad) | [✅](https://github.com/mamonaco1973/gcp-mini-ad) | [✅](https://github.com/mamonaco1973/azure-mini-ad) | [✅](https://github.com/mamonaco1973/oci-mini-ad) |
| Managed virtual desktops | [✅](https://github.com/mamonaco1973/aws-workspaces) | ✖️ | [✅](https://github.com/mamonaco1973/azure-virtual-desktops) | ✖️ |
| Linux remote desktops (xRDP) | [✅](https://github.com/mamonaco1973/aws-xubuntu-xrdp) | [✅](https://github.com/mamonaco1973/gcp-xubuntu-xrdp) | [✅](https://github.com/mamonaco1973/azure-xubuntu-xrdp) | [✅](https://github.com/mamonaco1973/oci-xubuntu-xrdp) |
| App auth (Cognito / Identity Platform / Entra) | [✅](https://github.com/mamonaco1973/aws-cognito-app) | [✅](https://github.com/mamonaco1973/gcp-identity-app) | [✅](https://github.com/mamonaco1973/azure-entra-app) | 🚧 |

### Networking & storage

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Hub-and-spoke networking | [✅](https://github.com/mamonaco1973/aws-transit-gateway) | [✅](https://github.com/mamonaco1973/gcp-mesh) | [✅](https://github.com/mamonaco1973/azure-wlan) | 🚧 |
| Shared file systems (EFS / Filestore / Files / FSS) | [✅](https://github.com/mamonaco1973/aws-efs) | [✅](https://github.com/mamonaco1973/gcp-filestore) | [✅](https://github.com/mamonaco1973/azure-nfs-files) | [✅](https://github.com/mamonaco1973/oci-fss) |
| Data migration | [✅](https://github.com/mamonaco1973/aws-data-sync) | 🚧 | 🚧 | 🚧 |

### Serverless

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Serverless CRUD API | [✅](https://github.com/mamonaco1973/aws-crud-example) | [✅](https://github.com/mamonaco1973/gcp-crud-example) | [✅](https://github.com/mamonaco1973/azure-crud-example) | 🚧 |
| Serverless MCP service | [✅](https://github.com/mamonaco1973/aws-serverless-mcp) | [✅](https://github.com/mamonaco1973/gcp-serverless-mcp) | [✅](https://github.com/mamonaco1973/azure-serverless-mcp) | 🚧 |
| Queue-driven workers (SQS / Pub/Sub / Service Bus) | [✅](https://github.com/mamonaco1973/aws-sqs-keygen) | [✅](https://github.com/mamonaco1973/gcp-pubsub-keygen) | [✅](https://github.com/mamonaco1973/azure-sb-keygen) | 🚧 |

### AI services

Applications built on each provider's native AI stack — vision, LLM, and agent services, not wrappers around a third-party API.

| Architecture | AWS | GCP | Azure | OCI |
|---|:---:|:---:|:---:|:---:|
| Cartoonify (vision AI image transformation) | [✅](https://github.com/mamonaco1973/aws-cartoonify) | [✅](https://github.com/mamonaco1973/gcp-cartoonify) | [✅](https://github.com/mamonaco1973/azure-cartoonify) | 🚧 |
| OpenClaw agent deployment | [✅](https://github.com/mamonaco1973/aws-openclaw) | [✅](https://github.com/mamonaco1973/gcp-openclaw) | [✅](https://github.com/mamonaco1973/azure-openclaw) | 🚧 |
| Resume app (LLM document processing) | [✅](https://github.com/mamonaco1973/aws-resume-app) | [✅](https://github.com/mamonaco1973/gcp-resume-app) | [✅](https://github.com/mamonaco1973/azure-resume-app) | 🚧 |

---

## How I work

- **Infrastructure as code, always** — Terraform/HCL first, console only for spelunking
- **Reference architectures over snowflakes** — patterns designed once, ported anywhere
- **AI-accelerated, human-verified** — I use AI tooling to compress build time from weeks to hours; ten years of architecture judgment is what makes the output trustworthy

---

*The pinned repos below are the best entry points, or the [YouTube channel](https://www.youtube.com/@MikesCloudSolutions) walks through the major builds end-to-end.*
