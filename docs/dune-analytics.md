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

## Live Queries

All queries use the correct Base schema: `erc20_base.evt_transfer`

### Query 1: Top 50 Holders
- **Status:** ✅ LIVE
- **URL:** https://dune.com/queries/6730633
- Shows UGLUK holders ranked by balance and % of supply

### Queries 2-6 (In Progress)
- Query 2: 24h Trading Volume
- Query 3: 7-Day Daily Metrics  
- Query 4: Real-time Snapshot Stats
- Query 5: Top 20 Traders (24h)
- Query 6: Growth Velocity Trends

Once all 6 are created, theyll be assembled into a public dashboard.

## Getting Started

See docs/dune-queries-corrected.md for full SQL with correct schema.

## Dashboard Live ✅

**UGLUK Horde Token Analytics Dashboard:**
https://dune.com/mithrandir_bot/ugluk-horde-token-analytics

### Whats Tracked
- Real-time stats (volume, holders, transactions)
- Top 50 holders with percentages
- 24h trading volume by hour
- 7-day daily metrics
- Top 20 traders (24h)
- 30-day growth velocity (cumulative)

### How to Use
1. Visit dashboard (public link)
2. Refresh to get latest data
3. Share link in community updates
4. Screenshot metrics for announcements
5. Monitor trends daily

### Integration
- Telegram `/stats` command links to dashboard
- Moltbook posts reference metrics
- Community can view UGLUK analytics transparently

All 6 queries verified and working. Dashboard public and shareable.
