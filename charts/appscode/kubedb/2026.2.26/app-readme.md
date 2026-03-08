## KubeDB by AppsCode — Database-as-a-Service (DBaaS) Anywhere with Any Storage

**KubeDB by AppsCode** is a certified, first-class Kubernetes operator delivering joint DBaaS
solutions for Rancher Prime environments across multi-cluster, multi-tenant, public/private cloud,
and air-gapped deployments.

Enterprises often struggle to deliver databases quickly while maintaining security, governance,
and operational control — forced to choose between restrictive cloud-managed services or complex
manual Kubernetes operations. KubeDB solves this by enabling platform teams to standardize and
govern production-ready databases across hybrid, multi-cloud, sovereign, and air-gapped
environments, while giving developers self-service access through Kubernetes-native workflows.

---

## Supported Databases

| Category | Engines |
|---|---|
| **Relational** | PostgreSQL, MySQL, MariaDB, Microsoft SQL Server, PerconaXtraDB |
| **NoSQL / Document** | MongoDB, FerretDB, Cassandra |
| **In-Memory / Cache** | Redis, Valkey, Memcached |
| **Search** | Elasticsearch, OpenSearch, Solr |
| **Analytics** | Druid, ClickHouse, SingleStore |
| **Messaging / Streaming** | Kafka, RabbitMQ |
| **In-Memory Data Grid** | Hazelcast, Ignite |
| **Coordination** | ZooKeeper |
| **Proxy / Pooler** | PgBouncer, Pgpool, ProxySQL |

---

## Features

### Provisioning and Lifecycle Management
Launch any database in minutes via CLI, API, or the self-service web portal — no ticket-based
provisioning required. Each database engine is defined as a Kubernetes Custom Resource (CRD),
so you use standard `kubectl`, Helm, or any Kubernetes-native tooling including GitOps (ArgoCD,
FluxCD). KubeDB automates the full lifecycle — provisioning, upgrades, scaling, failover, and
repair — through policy-driven declarative workflows, eliminating custom automation scripts and
manual operational risk. Custom database plugin support is available.

### Centralized Governance and Multi-Tenancy
Platform teams can enforce security policies, access controls, resource limits, and lifecycle
policies — enabling secure multi-tenant DBaaS at scale. KubeDB supports distributed environments
across clouds and data centers with centralized governance and local execution wherever
applications run.

### High Availability and Resiliency
KubeDB automatically replaces failed pods, performs continuous health checking, and uses
PodDisruptionBudgets during planned maintenance. Multi-AZ deployments replicate data to standby
instances across multiple Kubernetes failure domains, with placement zone control for data
affinity and governance requirements.

### Backup and Restore
Schedule backups at any frequency to cloud object stores (S3, GCS, Azure Blob, etc.) or local
filesystems (NFS, etc.). KubeDB uses KubeStash by AppsCode for incremental, deduplicated and
encrypted backups. One-off backups and on-demand restore to a new instance from any snapshot
are fully supported.

### Horizontal and Vertical Scaling
Scale database instances up or down — vertically (CPU/Memory) or horizontally (replicas) —
using a simple Kubernetes-native API without disrupting running workloads.

### Volume Expansion and Storage Flexibility
Dynamically expand persistent volumes without downtime. KubeDB works with existing enterprise
storage platforms and Kubernetes StorageClasses, giving organizations full data ownership while
optimizing for performance, resilience, and cost. Supports cloud-provider provisioned disks,
cloud-native storage solutions (Rook/Ceph, OpenEBS, Portworx via CSI, etc.), and local
persistent volumes for low-latency, high-throughput workloads.

### Version Upgrades
Automated upgrade workflows for all supported databases handle major, minor, and patch releases
with zero manual intervention.

### Monitoring and Alerting
Native Prometheus integration monitors all KubeDB-managed databases and the operator itself.
Use the built-in Prometheus scraper or Prometheus Operator. View key operational metrics —
compute, memory, storage utilization, I/O activity, and instance connections — via pre-built
Grafana dashboards. Prometheus Alertmanager routes event notifications to email, PagerDuty,
OpsGenie, and more. Third-party tools such as Datadog are also supported.

### Security
- **TLS/SSL management** — automated certificate provisioning and renewals for all database
  connections
- **Transparent Data Encryption (TDE)** - encrypted storage at rest via cloud provider key management services
- **Network isolation** — database pods run inside the Kubernetes private pod network by
  default; configurable network policies restrict communication to authorized pods only
- **RBAC resource-level permissions** — control which users and groups can act on specific
  database instances (e.g., developers on Dev, only DBAs on Prod)
- **Private registry and air-gapped cluster support** — runs fully offline with no internet
  access required; suitable for sovereign and regulated environments
- **Database user management** — Vault integration for dynamic credential generation,
  custom permissions, and automated credential rotation

### Cross-Cluster Access
Enable cross-cluster database access using Envoy Gateway — expose databases seamlessly across
cluster boundaries for multi-cluster and multi-region architectures.

### Single Operations Platform
Maintain one stack for all stateless and stateful workloads. Dev and ops teams share the same
tools, monitoring, logging, and alerting — no separate tooling for databases, no cloud lock-in,
the same workflows across on-premises, public cloud, sovereign, and air-gapped environments.

### Predictable Pricing
KubeDB follows an open-core model (API and client under Apache v2 License). A full 30-day trial
license is available free of cost. No up-front investment required.

---

## Supported Platforms

KubeDB integrates with any Kubernetes distribution, including:
**Rancher**, AWS EKS, Azure AKS, Google GKE, Red Hat OpenShift, VMware Tanzu, Equinix Metal,
OpenStack, IBM Cloud, Oracle Cloud, Alibaba Cloud, DigitalOcean, Akamai (Linode), Exoscale,
Hetzner Cloud, Kubermatic, Scaleway, and any on-premises Kubernetes cluster.

---

## More Information

- **Website:** https://kubedb.com
- **Documentation:** https://kubedb.com/docs
- **Features:** https://kubedb.com/features
- **Datasheet:** https://kubedb.com/datasheet
- **GitHub:** https://github.com/kubedb
- **Support:** https://appscode.freshdesk.com
- **Contact Sales:** https://appscode.com/contact
