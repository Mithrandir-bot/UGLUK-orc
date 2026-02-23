# UGLUK Analytics with Dune

Dune is the premier blockchain analytics platform for querying on-chain data.

## Why Dune for UGLUK?

- **Base mainnet indexed** (100+ blockchains supported)
- **Real-time data** (token transfers, swaps, holders)
- **SQL queries** (no coding experience needed)
- **Public dashboards** (transparent metrics for community)
- **API access** (power Telegram bot commands)

## Key Use Cases

### 1. Token Metrics Dashboard
- UGLUK price, volume, holders
- Trading activity trends
- Top traders leaderboard

### 2. Horde NFT Tracking
- NFT mint events
- Tier distribution (Member/Champion/Legend)
- Reward distribution

### 3. Community Analytics
- New vs active users
- Holding patterns
- Engagement metrics

### 4. Raid Performance
- Coordinated buying analysis
- Impact measurement
- Success prediction

## Getting Started

1. **Create Account:** https://app.dune.com/auth/register
2. **Explore Base:** Query blockchain data with SQL
3. **Write Queries:** Use provided examples
4. **Create Dashboard:** Visualize results
5. **Share Publicly:** Link in community

## Sample Query

```sql
-- UGLUK Token Holders
SELECT 
  to AS holder,
  SUM(value) / 1e18 AS balance
FROM base.token_transfers
WHERE contract_address = 0x5e9f156fB9beB0b4F3Ffc0F47ba1b1CE79f40383
GROUP BY to
ORDER BY balance DESC
LIMIT 20;
```

## API Integration

Access Dune data programmatically:
- Execute queries via API
- Get results in JSON
- Power Telegram bot commands
- Build real-time dashboards

## Resources

- **Docs:** https://docs.dune.com/
- **API Ref:** https://docs.dune.com/api-reference/
- **Community:** https://dune.com/browse/dashboards

---

Transparent metrics for a transparent token. 🦞
