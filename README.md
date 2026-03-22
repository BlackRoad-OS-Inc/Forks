# Road Fleet Forks

Registry of 65 open-source dependencies. Each one forked, named, assigned to a node, and deployed from our infrastructure.

## What This Is

Every critical dependency is forked into this organization instead of pulled from upstream at deploy time. Each fork gets a Road name, a node assignment, and runs from our copy. This repo is the registry.

## Core Fleet

| Road Name | Upstream | Deployed On | Purpose |
|-----------|----------|-------------|---------|
| **RoadCode** | Gitea | Octavia | Git hosting (239 repos) |
| **TollBooth** | WireGuard | All 7 nodes | VPN mesh |
| **PitStop** | Pi-hole | Alice | DNS filtering |
| **Passenger** | Ollama | 4 nodes | Local AI inference |
| **OneWay** | Caddy | Gematria | TLS edge proxy |
| **RearView** | Qdrant | Alice | Vector search |
| **Curb** | MinIO | Cecilia | Object storage |
| **RoundAbout** | Headscale | Octavia | Mesh coordination |
| **CarPool** | NATS | Octavia | Message bus |
| **OverPass** | n8n | Octavia | Workflow automation |
| **BackRoad** | Portainer | Octavia | Container management |
| **RoadMap** | Grafana | Alice | Fleet monitoring |

Plus 53 additional forks covering databases, runtimes, DNS, TLS, CI/CD, and media.

## Why Fork Everything

1. **No surprise breakage** — upstream changes do not hit production without review
2. **Audit trail** — every change tracked in your git history
3. **Availability** — if upstream disappears, you still have the code
4. **Customization** — patches stay clean, rebases are intentional

## Updating a Fork

```bash
git remote add upstream <original-repo-url>
git fetch upstream
git log upstream/main --oneline -20    # Review what changed
git merge upstream/main                # Merge when ready
```

Updates are pulled manually after review. No automatic sync from upstream.

## Infrastructure

- **5 Raspberry Pis**: Alice, Cecilia, Octavia, Aria, Lucidia
- **2 cloud servers**: Gematria (edge), Anastasia
- **7-node mesh** connected via WireGuard (TollBooth)

## License

Proprietary. Copyright (c) 2024-2026 BlackRoad OS, Inc. All rights reserved.

Individual forks retain their original upstream licenses. The registry, Road naming, deployment configs, and customizations are proprietary.

---

*Remember the Road. Pave Tomorrow.*
