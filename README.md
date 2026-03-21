# BlackRoad Road Fleet — Sovereign Forks

> Every dependency we use, we own. Fork it, brand it, deploy it, control it.

**BlackRoad OS, Inc.** — Delaware C-Corp, founded November 17, 2025.

## Road Fleet Registry

| Road Name | Upstream | Status | Deployed On | Purpose |
|-----------|----------|--------|-------------|---------|
| **TollBooth** | WireGuard | LIVE | All 7 nodes | Encrypted VPN mesh |
| **PitStop** | Pi-hole | LIVE | Alice | DNS filtering, ad blocking |
| **Passenger** | Ollama | LIVE | 4 nodes | Local AI inference engine |
| **OneWay** | Caddy | LIVE | Gematria | TLS edge, reverse proxy |
| **RearView** | Qdrant | LIVE | Alice | Vector DB, semantic search |
| **Curb** | MinIO | LIVE | Cecilia | S3-compatible object storage |
| **RoundAbout** | Headscale | LIVE | Octavia | VPN coordination |
| **CarPool** | NATS | LIVE | Octavia | Pub/sub messaging |
| **OverPass** | n8n | LIVE | Octavia | Workflow automation |
| **BackRoad** | Portainer | LIVE | Octavia | Container management |
| **RoadMap** | Grafana | LIVE | Aria | Monitoring dashboards |
| **RoadCode** | Gitea | LIVE | Octavia :3100 | Git hosting (239 repos) |
| **RoadBase** | PostgreSQL | LIVE | Alice, Cecilia | Relational database |
| **RoadCache** | Redis | LIVE | Alice | In-memory cache |
| **RoadPulse** | InfluxDB | LIVE | Cecilia | Time-series metrics |
| **RoadLite** | SQLite | LIVE | Everywhere | Embedded database |
| **RoadVoice** | Whisper | NEW | — | Speech-to-text |
| **RoadLlama** | llama.cpp | NEW | — | C++ LLM inference |
| **RoadRunner** | act_runner | NEW | Octavia | CI/CD runner |
| **RoadProcess** | pm2 | LIVE | Alice, Octavia | Process manager |
| **RoadProxy** | nginx | LIVE | Alice, Lucidia | Reverse proxy |
| **RoadDNS** | PowerDNS | LIVE | Lucidia, Gematria | Authoritative DNS |
| **RoadTunnel** | cloudflared | LIVE | Alice | Tunnel client |
| **RoadWatch** | Prometheus | NEW | — | Metrics collection |
| **RoadLight** | Uptime Kuma | NEW | — | Uptime monitoring |
| **RoadGuard** | fail2ban | LIVE | Alice | Intrusion prevention |
| **RoadShield** | CrowdSec | NEW | — | Threat intelligence |
| **RoadCert** | certbot | LIVE | Gematria | TLS automation |
| **RoadChat** | Matrix/Element | NEW | — | Sovereign messaging |
| **RoadDraw** | Excalidraw | NEW | — | Collaborative whiteboard |
| **RoadDocs** | HedgeDoc | NEW | — | Collaborative docs |
| **RoadMetrics** | Plausible | NEW | — | Privacy-first analytics |
| **RoadLearn** | Moodle | NEW | — | Learning management |
| **RoadCodec** | FFmpeg | NEW | — | Video processing |
| **RoadStream** | Jellyfin | NEW | — | Media server |
| **RoadTube** | PeerTube | NEW | — | Video hosting |
| **RoadCanvas** | Stable Diffusion | NEW | — | Image generation |

## Architecture

```
Internet → Gematria (OneWay/Caddy) → WireGuard (TollBooth) → Pi Fleet
                                                                ├── Alice (RoadProxy, PitStop, RoadBase, RoadCache, RearView)
                                                                ├── Cecilia (Passenger/Ollama, Curb/MinIO, RoadPulse)
                                                                ├── Octavia (RoadCode/Gitea, CarPool/NATS, BackRoad/Docker)
                                                                ├── Aria (RoadMap/Grafana)
                                                                └── Lucidia (RoadProxy, RoadDNS)
```

## Why Fork Everything?

1. **Sovereignty** — No vendor can pull the rug. We control our stack.
2. **Customization** — Each fork is branded and optimized for BlackRoad fleet.
3. **Security** — We audit and patch on our timeline, not upstream's.
4. **Identity** — Road Fleet names create a cohesive ecosystem language.
5. **Resilience** — If upstream dies, we keep running.

## Fork Standards

Every Road Fleet fork must:
- [ ] Be forked to `BlackRoad-OS-Inc/<RoadName>`
- [ ] Have a BlackRoad-branded README with Road Fleet branding
- [ ] Include `RoadCode/` directory with `roadcode.json`
- [ ] Include `LICENSE` (proprietary BlackRoad OS, Inc.)
- [ ] Include `TODO.md` and `ROADMAP.md`
- [ ] Be deployed on at least one Pi fleet node
- [ ] Be registered in the backend API (`backend.blackroad.io/api/repos`)

## Infrastructure

- **5 Raspberry Pis**: Alice, Cecilia, Octavia, Aria, Lucidia
- **2 DigitalOcean droplets**: Gematria (edge), Anastasia (cloud)
- **52 TOPS** AI acceleration (2x Hailo-8)
- **WireGuard mesh**: 7 nodes, 12 connections
- **239 repos** on Gitea (Octavia :3100)

---

**BlackRoad OS — Remember the Road. Pave Tomorrow.**

*Proprietary. BlackRoad OS, Inc. All rights reserved.*
