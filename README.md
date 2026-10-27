<a href="https://hetops.dev"><img src="https://cdn.jsdelivr.net/gh/Het101/hetops-portfolio@main/assets/og.png" alt="HetOps: I turn production incidents into tools. Het Patel, DevOps Engineer II, hetops.dev" width="100%" /></a>

# Het Patel

DevOps Engineer II at **Techdome**, Mumbai. Multi-cloud Kubernetes at work, open-source tools for everyone else.
Every tool below started as a real production problem.

[hetops.dev](https://hetops.dev) · [Résumé](https://hetops.dev/Het_Patel_Resume.pdf) · [LinkedIn](https://linkedin.com/in/het-patel-101) · [patel.x.het@gmail.com](mailto:patel.x.het@gmail.com)

## Three years in numbers

- **$2M a year** saved by cost automation that finds idle cloud resources and right-sizes the rest
- **100+ nodes, 3 clouds**: one control plane across AWS, GCP and Azure, with automated failover
- **10K deploys**: canary releases with automated rollback, through GitOps
- **60% faster deploys, 99.9% uptime**: CI/CD, Kubernetes and observability at DataGrokr
- **7,200 threads**: a broken chat migration repaired with every author kept; it became Threadvault

## Tools I built from incidents

| Tool | The problem it answers | Run it |
|---|---|---|
| [**Threadvault**](https://github.com/Het101/threadvault) | A chat migration broke 7,200 threads. Mirror Azure Communication Services or Twilio into your own Postgres, then migrate, replay and verify. | `npx threadvault doctor` <br> [![npm](https://img.shields.io/npm/dm/threadvault?style=flat-square&label=installs)](https://www.npmjs.com/package/threadvault) |
| [**Retirement Radar**](https://github.com/Het101/retirement-radar) | AWS bills extra for old versions; EKS extended support alone is about $365 a month per cluster. Scans every region for EOL EKS, RDS, ElastiCache, OpenSearch, MSK and Lambda. | `npx retirement-radar scan` <br> [![npm](https://img.shields.io/npm/dm/retirement-radar?style=flat-square&label=installs)](https://www.npmjs.com/package/retirement-radar) |
| [**Radar Cloud**](https://radar.hetops.dev) | The same scan on a schedule, across every account, through a read-only role, with Slack and email alerts. | [![Radar Cloud](https://status.hetops.dev/api/badge/6/status?style=flat-square&label=radar.hetops.dev)](https://radar.hetops.dev) |
| [**DNS Intelligence**](https://dns.hetops.dev) | An SPF record past 10 lookups fails, and nested includes hide the count. 26 checks across DNS, TLS, headers, DNSSEC and email auth. | [![DNS Intelligence](https://status.hetops.dev/api/badge/5/status?style=flat-square&label=dns.hetops.dev)](https://dns.hetops.dev) |
| [**Restore Drill**](https://github.com/Het101/restore-drill) | A backup job that says "success" proves nothing. Every six hours it restores the newest offsite backup into a throwaway copy and checks it. | [![Restore Drill](https://status.hetops.dev/api/badge/12/status?style=flat-square&label=backups%20restore-tested)](https://drill.hetops.dev) |

The badges are live, from [status.hetops.dev](https://status.hetops.dev).

## Break my Kubernetes lab

[**hetops.dev/lab**](https://hetops.dev/lab) lets anyone kill pods, drop the database or flood the API of a real multi-tenant app. Kubernetes and Argo CD heal it while you watch, and an error budget freezes the chaos when it has done enough damage.

Under it: kubeadm on Oracle Cloud ARM, Argo CD app-of-apps, Linkerd mTLS, NGINX Gateway Fabric, Sealed Secrets, cert-manager, Prometheus SLOs with Telegram alerts, ELK, Falco, and CrowdSec feeding Cloudflare's WAF. The host layer is Ansible ([Bedrock](https://github.com/Het101/hetops-k8s-lab/tree/main/bedrock)): every server change and Kubernetes upgrade lands on a staging VM first, and CI rebuilds the node from a blank image every week.

[![Bedrock](https://github.com/Het101/hetops-k8s-lab/actions/workflows/bedrock.yml/badge.svg)](https://github.com/Het101/hetops-k8s-lab/actions/workflows/bedrock.yml)

## How I ship

`test` → `hygiene` → `analyze` → `stage` → `approve`

Nothing reaches main until all five pass, and nothing reaches npm until a human approves it with 2FA. Signed commits, linear history, Actions pinned to a commit, CodeQL, Trivy and Semgrep in CI.

## Stack

<a href="https://hetops.dev"><img src="https://skillicons.dev/icons?i=kubernetes,terraform,ansible,docker,aws,gcp,azure,githubactions,prometheus,grafana,elasticsearch,nginx,cloudflare,linux,bash,py,ts&perline=17" alt="Kubernetes, Terraform, Ansible, Docker, AWS, GCP, Azure, GitHub Actions, Prometheus, Grafana, Elasticsearch, NGINX, Cloudflare, Linux, Bash, Python, TypeScript" /></a>

Also Helm, Argo CD, Linkerd, Falco, CrowdSec, Vault, Trivy, OpenTelemetry and Oracle Cloud.

---

Off the clock I'm an otaku. Also on [Instagram](https://instagram.com/_.imhet) and [Discord](https://discord.gg/EdaEA86GTj).
