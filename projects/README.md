# Qloudex project directory

This directory describes the public engineering projects associated with
Qloudex. The entries below are based on currently visible source, documentation,
and configuration. They are not customer case studies or claims of production
deployment.

Maturity labels are descriptive:

- **Active experiment** — substantial implementation intended for continued
  engineering and evaluation.
- **Beta** — implemented workflows with documented readiness limits.
- **Reference project** — a runnable or inspectable example intended primarily
  for learning and demonstration.
- **Learning reference** — environment-specific examples that require
  adaptation before use.

## KubePilot

**Repository:** [Qloudex/kubepilot](https://github.com/Qloudex/kubepilot)  
**Maturity:** Active experiment

### Purpose

KubePilot is a Kubernetes operations assistant for asking operational questions,
retrieving relevant runbooks, inspecting workload evidence, diagnosing common
deployment failures, and generating incident reports.

### Verified technologies

- Python 3.11+, FastAPI, pytest, and Ruff
- Go Kubernetes inspection service
- Markdown retrieval with optional FAISS vector search
- Optional LangGraph workflow mode
- Docker Compose and a static browser console
- Helm and Argo CD deployment assets
- Prometheus, Grafana, audit events, and optional OpenTelemetry integration

### Current limitations

- The deterministic local fixture demo is the easiest verified starting point.
- Real-cluster permissions, identity, secrets, and observability need
  environment-specific configuration and review.
- Production readiness is documented as incomplete; remediation remains
  approval-gated.
- No license file is currently present in the Qloudex repository.

## SystemMonitoring

**Repository:** [Qloudex/SystemMonitoring](https://github.com/Qloudex/SystemMonitoring)  
**Maturity:** Reference project

### Purpose

SystemMonitoring demonstrates a containerized FastAPI application instrumented
for Prometheus and visualized through provisioned Grafana dashboards.

### Verified technologies

- Python, FastAPI, Uvicorn, and Prometheus FastAPI Instrumentator
- Prometheus and Grafana
- Docker and Docker Compose
- pandas and scikit-learn utilities for offline recommendation experiments
- Python tests and GitHub Actions workflow definitions

### Current limitations

- The FastAPI service exposes root, health, and metrics behavior; the offline
  recommendation utilities are not integrated into the monitoring API.
- Several Python dependencies are pinned to older versions.
- The Compose configuration uses default Grafana credentials and floating
  Prometheus/Grafana image tags, so it is not a production configuration.
- The Qloudex fork shows workflow definitions but no organization workflow runs
  were available during the documentation audit.
- No license file is currently present in the Qloudex repository.

## Codewise CLI

**Repository:** [Qloudex/Codewise-CLI](https://github.com/Qloudex/Codewise-CLI)  
**Maturity:** Beta

### Purpose

Codewise CLI provides a Go command surface for scaffolding and operating common
Docker, Kubernetes, Helm, deployment, environment, configuration, template, and
file-conversion workflows.

### Verified technologies

- Go and Cobra
- Docker, kubectl, Kubernetes, and Helm integrations
- Environment-aware deployment planning, status, logs, history, and rollback
  commands
- YAML, JSON, TOML, XML, ENV, and Base64 conversion utilities
- Go tests, kind-based end-to-end workflow, and GitHub Actions definitions
- VitePress documentation

### Current limitations

- The project describes itself as beta and requires a production-readiness
  review before use with important workloads.
- Several commands depend on external tools and a correctly configured cluster.
- The Qloudex fork does not currently publish its own release artifacts; the
  documented verified releases belong to the upstream repository.
- The repository is licensed under Apache License 2.0.

## GO-CI-CD

**Repository:** [Qloudex/GO-CI-CD](https://github.com/Qloudex/GO-CI-CD)  
**Maturity:** Learning reference

### Purpose

GO-CI-CD pairs a small Go web application with example OpenShift delivery
resources covering Tekton tasks, Buildah image creation, Kubernetes/OpenShift
deployment, and Argo CD synchronization.

### Verified technologies

- Go 1.22 and Martini
- Go unit and HTTP handler tests
- Dockerfile based on the Red Hat UBI Go toolset
- OpenShift, Tekton, Buildah, and Argo CD manifests

### Current limitations

- Manifests contain cluster-specific registry, namespace, route, and repository
  values that must be replaced.
- The pipeline passes a parameter named `url`, while the referenced clone task
  declares `repo-url`; the example needs correction before execution.
- The GitHub Actions workflow is commented out and does not currently run CI.
- README screenshots referenced by the upstream documentation are not present in
  the Qloudex repository tree.
- No license file is currently present in the Qloudex repository.

## Licensing and attribution

Each project retains its own Git history, upstream relationship, attribution,
and license status. The [MIT license](../LICENSE) for the Qloudex project hub
does not grant a license for a linked repository that has no license file.
