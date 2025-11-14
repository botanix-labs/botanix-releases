# Botanix Public Releases

This repository contains public release artifacts, documentation, and changelogs for Botanix.

## Latest Releases

| Channel | Version | Release Date | Downloads |
|---------|---------|--------------|-----------|
| stable | 1.5.2 | | [Download](releases/1.5.2) |

## Quick Start

### Docker (Recommended)
```bash
# Use explicit version tags for reproducible builds
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.5.2
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.5.2
```

### Binary Installation
```bash
# Download stable binaries with explicit version
curl -L https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.5.2/reth-x86_64-unknown-linux-gnu.tar.gz | tar -xz
curl -L https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.5.2/btc-server-x86_64-unknown-linux-gnu.tar.gz | tar -xz
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
