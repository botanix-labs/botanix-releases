# Botanix Public Releases

This repository contains public release artifacts, documentation, and changelogs for Botanix.

## Latest Releases

| Channel | Version | Release Date | Downloads |
|---------|---------|--------------|-----------|
| hotfix | 1.1.14-hotfix.3 | | [Download](releases/1.1.14-hotfix.3) |

## Quick Start

### Docker (Recommended)
```bash
# Latest stable release
docker pull ghcr.io/botanix-labs/botanix-reth-node:latest
docker pull ghcr.io/botanix-labs/botanix-btc-server:latest

# Development builds
docker pull ghcr.io/botanix-labs/botanix-reth-node:alpha
docker pull ghcr.io/botanix-labs/botanix-btc-server:alpha
```

### Binary Installation
```bash
# Download latest stable binaries
curl -L https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/latest/reth-x86_64-unknown-linux-gnu.tar.gz | tar -xz
curl -L https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/latest/btc-server-x86_64-unknown-linux-gnu.tar.gz | tar -xz
```

## Documentation

- [Release Notes](releases/) - Detailed release information
- [Changelogs](changelog/) - Version history by channel

## Channels

- **stable** (latest) - Production-ready releases
- **rc** - Release candidates for testing
- **alpha** - Development builds with latest features
- **hotfix** - Emergency fixes for production issues

## Support

- [GitHub Issues](https://github.com/botanix-labs/botanix-releases/issues)
- [Documentation](https://github.com/botanix-labs/documentation)

---

*This repository is automatically updated by the release pipeline.*
