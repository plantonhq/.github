# DevOps Infrastructure as Open Source

<div align="center">

**Deploy production infrastructure in minutes, not weeks.**

[![Website](https://img.shields.io/badge/Website-planton.ai-7c3aed?style=for-the-badge)](https://planton.ai)
[![Console](https://img.shields.io/badge/Console-console.planton.ai-0ea5e9?style=for-the-badge)](https://console.planton.ai)
[![License](https://img.shields.io/badge/License-Apache%202.0-10b981?style=for-the-badge)](https://github.com/plantonhq/project-planton/blob/main/LICENSE)

**120+ Deployment Components** • **450+ Production Deployments** • **100% Customer Retention**

</div>

---

## 🚀 What is Planton?

Planton combines **open source infrastructure modules** with a **commercial orchestration platform** to eliminate DevOps bottlenecks.

### Project Planton (Open Source)
- **120+ Terraform & Pulumi deployment modules** for AWS, GCP, Azure, DigitalOcean, Civo, Cloudflare
- **CLI tools** for local infrastructure management (`project-planton`)
- **Schema definitions** and validation rules (Protocol Buffers)
- **All code public and auditable** at [github.com/plantonhq/project-planton](https://github.com/plantonhq/project-planton)

### Planton Cloud (Commercial Platform)
- **SaaS orchestration** layer that runs the open source modules
- **Service Hub** for backend CI/CD (Tekton-powered)
- **AI Agents** for DevOps automation (Beta)
- **Multi-cloud management** without vendor lock-in

**The Difference**: With Terraform Cloud or Pulumi Cloud, *you write and maintain modules yourself*. With Planton, we provide 120+ production-ready modules that you can audit, fork, or use independently.

---

## 📦 Open Source Deployment Components

All infrastructure modules are **100% open source**. Audit every line of code, fork for customization, or use independently of the platform.

### Cloud Infrastructure
- **Networking**: VPC, Subnets, NAT Gateways, Route Tables
- **DNS & Certificates**: Route53, Cloud DNS, ACM, Let's Encrypt
- **Load Balancing**: ALB, NLB, Cloud Load Balancer, Application Gateway

### Container Platforms
- **AWS**: ECS, EKS, App Runner
- **GCP**: GKE, Cloud Run, Artifact Registry
- **Azure**: AKS, Container Apps, Container Registry
- **Kubernetes**: Standard K8s deployments across any provider

### Databases & Storage
- **Relational**: PostgreSQL, MySQL, Aurora, Cloud SQL
- **NoSQL**: MongoDB, DynamoDB, Firestore, Cosmos DB
- **Caching**: Redis, Memcached, Elasticache
- **Object Storage**: S3, GCS, Azure Blob Storage

### Queues & Streaming
- **Message Queues**: SQS, Pub/Sub, Service Bus, RabbitMQ
- **Event Streaming**: Kafka, Kinesis, Event Hubs

### Quick Start

```bash
# Install CLI
brew install project-planton/tap/project-planton

# Deploy AWS ECS environment
planton chart install aws-ecs \
  --name api \
  --env prod \
  --values values.yaml

# Output:
# ✓ VPC created (3m 12s)
# ✓ Load Balancer configured (4m 45s)
# ✓ ECR registry ready (1m 30s)
# ✓ SSL certificates issued (2m 15s)
# ✓ DNS configured (1m 8s)
# ⚡ Complete in 12 minutes
```

---

## 🏗️ Built on Open Standards

No proprietary formats. No vendor lock-in by design.

| Standard | Technology | Why |
|----------|-----------|-----|
| **IaC** | Terraform & Pulumi | Not a custom DSL—use the tools you know |
| **CI/CD** | Tekton (CNCF Graduated) | Kubernetes-native, portable, extensible |
| **Git** | GitHub & GitLab | OAuth integration, existing workflows |
| **Containers** | Docker & Kubernetes | Standard OCI images, vanilla K8s resources |
| **Schemas** | Protocol Buffers | Language-agnostic validation and code generation |

**Exit Strategy Built-In**:
1. Export all configurations as YAML manifests (one API call)
2. Use `project-planton` CLI independently from your own CI/CD
3. Fork and modify any deployment module on GitHub
4. Migrate to GitHub Actions using exported Tekton pipelines

---

## 📚 Key Repositories

| Repository | Description | Status |
|------------|-------------|--------|
| [project-planton/project-planton](https://github.com/plantonhq/project-planton) | Main monorepo with 120+ deployment components | ⭐ Active |
| [plantonhq/homebrew-tap](https://github.com/plantonhq/homebrew-tap) | Homebrew formulae for CLI installation | 🍺 Maintained |
| [plantonhq/infra-charts](https://github.com/plantonhq/infra-charts) | Infrastructure orchestration charts | 📦 Active |
| [plantonhq/tekton-hub](https://github.com/plantonhq/tekton-hub) | Tekton pipeline catalog | 🔧 Active |

---

## 🤝 Community & Contributing

We welcome contributions to deployment modules, CLI tools, and documentation!

- **💬 Community Discussions**: [GitHub Discussions](https://github.com/orgs/plantonhq/discussions) (coming soon)
- **🐛 Report Issues**: File issues in respective repositories
- **📖 Documentation**: [docs.planton.ai](https://docs.planton.ai) (coming soon)
- **🎯 Good First Issues**: Look for `good-first-issue` labels across repos

### How to Contribute
1. Fork the repository
2. Create a feature branch
3. Make your changes with tests
4. Submit a pull request
5. Celebrate 🎉

---

## 🎯 Are You a...

<table>
<tr>
<td width="50%">

### 👨‍💻 User?
**Want to deploy infrastructure without the wait?**

- 🚀 [Try Planton Cloud](https://console.planton.ai) (100 free automation minutes)
- 📖 [Read the Docs](https://planton.ai) 
- 🎥 [Watch 5-Min Demo](https://docs.google.com/forms/d/17tEVBbpIGl0AR4M75IOBYj4Ywap1RPCzZc4HMWA-67U)
- 💰 [See Pricing](https://planton.ai/#pricing)

**Starting at $20/developer/month**

</td>
<td width="50%">

### 🛠️ Contributor?
**Want to improve open source DevOps tooling?**

- ⭐ [Star project-planton](https://github.com/plantonhq/project-planton)
- 🍴 [Fork and modify modules](https://github.com/plantonhq/project-planton)
- 🐛 [Report bugs or request features](https://github.com/plantonhq/project-planton/issues)
- 📝 [Read contribution guidelines](https://github.com/plantonhq/project-planton/blob/main/CONTRIBUTING.md)

**All deployment modules are Apache 2.0**

</td>
</tr>
</table>

---

## 🌟 Why Planton?

| Feature | Terraform Cloud | Pulumi Cloud | Planton |
|---------|-----------------|--------------|---------|
| **Setup Time** | 1-2 days | 1-2 days | <1 hour |
| **Monthly Cost** (7 devs) | $1,200+ | $1,000+ | $450 |
| **Backend CI/CD** | ❌ Build yourself | ❌ Build yourself | ✅ Included (Tekton) |
| **Out-of-the-box Infra** | ❌ Write all modules | ⚠️ Limited components | ✅ 120+ components |
| **CLI Open Source** | ✅ Yes | ✅ Yes | ✅ Yes |
| **Deployment Modules Open Source** | ❌ You write your own | ❌ You write your own | ✅ All 120+ on GitHub |
| **Platform (SaaS) Open Source** | ❌ Proprietary | ❌ Proprietary | ❌ Proprietary |
| **Exit Strategy** | ⚠️ Migration cost | ⚠️ Migration cost | ✅ Export everything |

**Real Customer Results**:
- **<1 hour** infrastructure deployment (vs. weeks manual)
- **96% cost reduction** vs. hiring DevOps engineer
- **100% customer retention** since launch
- **450+ production deployments** completed

---

## 📬 Connect With Us

- 🌐 **Website**: [planton.ai](https://planton.ai)
- 🖥️ **Platform**: [console.planton.ai](https://console.planton.ai)
- 🐙 **GitHub**: [@plantonhq](https://github.com/plantonhq)
- 🐦 **Twitter**: [@plantonhq](https://twitter.com/plantonhq)
- 💼 **LinkedIn**: [plantoncloud](https://linkedin.com/company/plantoncloud)

---

<div align="center">

**Built by DevOps engineers who felt the pain.**

*Use Planton because it's the best platform—not because switching is too expensive.*

[![License](https://img.shields.io/badge/License-Apache%202.0-10b981)](https://github.com/plantonhq/project-planton/blob/main/LICENSE)
[![Multi-Cloud](https://img.shields.io/badge/Multi--Cloud-AWS%20%7C%20GCP%20%7C%20Azure-7c3aed)](https://planton.ai)
[![Open Source](https://img.shields.io/badge/Open%20Source-120%2B%20Modules-0ea5e9)](https://github.com/plantonhq/project-planton)

</div>

