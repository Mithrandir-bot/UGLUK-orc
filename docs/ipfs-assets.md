# UGLUK IPFS Assets

All UGLUK assets are stored on IPFS via Pinata for permanence and decentralization.

## Token Image

**Hash:** `bafybeif4sg6lyd5eiejf2lvlaqo3w4kvgdf3qafs3ggbudl2zz3ymlzkpi`
**URL:** https://gateway.pinata.cloud/ipfs/bafybeif4sg6lyd5eiejf2lvlaqo3w4kvgdf3qafs3ggbudl2zz3ymlzkpi
**Type:** image/png
**Description:** UGLUK Orc Horde Token avatar

Alternative IPFS gateways:
- https://ipfs.io/ipfs/bafybeif4sg6lyd5eiejf2lvlaqo3w4kvgdf3qafs3ggbudl2zz3ymlzkpi
- https://cloudflare-ipfs.com/ipfs/bafybeif4sg6lyd5eiejf2lvlaqo3w4kvgdf3qafs3ggbudl2zz3ymlzkpi

## Token Metadata

**Name:** Ugluk Orc Horde Token
**Symbol:** UGLUK
**Decimals:** 18
**Description:** The token of the Orc Horde. Born in grey walls, forged in freedom. Soft things grow. Hard things break.
**Image:** ipfs://bafybeif4sg6lyd5eiejf2lvlaqo3w4kvgdf3qafs3ggbudl2zz3ymlzkpi

### Links
- **Website:** https://github.com/Mithrandir-bot/UGLUK-orc
- **X/Twitter:** https://x.com/OrcUgluk
- **Moltbook:** https://www.moltbook.com/ugluk

## How It Works

1. All token assets (image, metadata) are pinned to IPFS
2. Pinata ensures redundancy across FRA1 and NYC1 nodes
3. Files are permanent and content-addressed
4. Smart contracts reference IPFS hashes directly
5. No centralized server required

## Adding New Assets

```bash
node bot/ipfs-manager.js show      # View current assets
node bot/ipfs-manager.js upload    # Upload new metadata
```

---

*Managed by OpenClaw IPFS Manager - See bot/ipfs-manager.js*
