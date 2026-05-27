# Platform & AI Engineer

12+ years in infrastructure, platform engineering, and operations. Currently building at the intersection of bare-metal infrastructure and AI agent systems.

I run a multi-node Kubernetes cluster on Proxmox that hosts 50+ applications, including AI-powered platforms I've built from scratch. Everything is GitOps-managed, Terraform-provisioned, and monitored end-to-end.

## Current Focus

**[agents-platform](https://github.com/kernelpanic09/agents-platform)** -- An AI agent orchestration platform with RAG (Qdrant + Ollama), LangGraph workflows, cost/latency observability, and LLM evaluation. 26 agent personas that dispatch via SSH to Claude Code for real infrastructure tasks. Built with Node.js, React, LangChain, and SQLite.

**Bare-Metal K3s** -- 3-node cluster on Proxmox running 50+ workloads with ArgoCD (GitOps), Longhorn (distributed storage), MetalLB (load balancing), Traefik (ingress), and Prometheus/Grafana (observability). Every app deploys through a single `deploy.sh` that builds, pushes, and syncs automatically.

**Infrastructure as Code** -- Terraform modules for Proxmox VM provisioning with cloud-init templating. Ansible for OS bootstrapping and cluster maintenance. Pi-hole DNS (HA pair), WireGuard VPN, pfSense firewall.

## Stack

```
Platform        K3s · Proxmox · ArgoCD · Traefik · MetalLB · Longhorn · Helm
Infrastructure  Terraform · Ansible · cloud-init · pfSense · WireGuard · Pi-hole
AI Engineering  LangChain · LangGraph · Qdrant · Ollama · Claude API · MCP
Languages       JavaScript/TypeScript · Python · HCL · Bash · Go
Cloud           AWS (Organizations, Identity Center, S3, IAM) · GitHub Actions
Observability   Prometheus · Grafana · Uptime Kuma · Custom telemetry
```

## How I Work

I build things that run on real hardware, serve real traffic, and break in real ways. The systems I operate handle storage failures, node reboots, DHCP lease changes, and USB passthrough race conditions -- not just happy-path demos.

I treat AI agents the same way I treat infrastructure: if you can't observe it, schedule it, evaluate it, and recover from its failures, it's not production-ready.

Every project ships with IaC, GitOps manifests, monitoring, and a one-command deploy pipeline. The gap between "it works on my machine" and "it runs in production" is where I spend most of my time.

---

`USA` · `kernelpanic09`
