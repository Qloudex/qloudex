# Qloudex

Agentic AI for software, data and cloud automation.

Qloudex helps companies and developers automate software development, data platforms and cloud infrastructure tasks using agentic AI, data engineering, RAG pipelines and DevOps tools. We are an early-stage, open-source initiative by two developers.

## Why agentic AI + DevOps

Most engineering time on infrastructure goes to repetitive diagnosis: why is this pod restarting, why did this pipeline fail, what changed. An agent that can read the error, form a hypothesis, run the right diagnostic commands and explain the result saves real time. We combine that with solid DevOps practice (containers, Kubernetes, IaC, CI/CD, monitoring) so the tools are deployable, not just demos.

## What we are building

- AI agents for Kubernetes, Docker and CI/CD troubleshooting
- Tooling that connects agents to real infrastructure workflows (GitOps, observability)
- Reference implementations: agent, container, Kubernetes, Terraform, CI/CD and monitoring

## Current projects

| Project | Status | Description |
|---|---|---|
| [kubepilot](https://github.com/AryanSharma9917/kubepilot) | Active | AI Kubernetes and DevOps copilot with RAG, tool-calling, GitOps workflows and observability |
| [SystemMonitoring](https://github.com/AryanSharma9917/SystemMonitoring) | Active | FastAPI + Prometheus + Grafana with AI-driven recommendations |
| [Codewise-CLI](https://github.com/AryanSharma9917/Codewise-CLI) | Active | DevOps CLI utilities |

Projects are moving into this organization; links will be updated.

## Repository layout

```
docs/       Documentation and architecture notes
projects/   Index of Qloudex projects
examples/   Usage examples and sample configs
```

## Roadmap

- [ ] Move core projects into the organization
- [ ] Documentation for each project: problem, how it works, how to run it, examples, architecture
- [ ] Dockerfile, Kubernetes manifests and Helm chart for the flagship agent
- [ ] CI/CD pipeline and Terraform example
- [ ] Monitoring and logging for deployed agents
- [ ] Technical articles and demos

## Contributing

We welcome issues and pull requests. Read [CONTRIBUTING.md](CONTRIBUTING.md) to get started.

## Team

Aryan Sharma and Rakshit Sharma, co-founders and builders.

## License

MIT. See [LICENSE](LICENSE).
