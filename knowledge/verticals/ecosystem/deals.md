---
type: context-summary
domain: deals
refreshed: 2026-03-02
---

# Deals & Partners

## Active / Strategic Integrations

| Partner | Product | Status | Priority | Key Contact | Notes |
|---------|---------|--------|----------|-------------|-------|
| Figure Markets | YLDS + tokenized equity on Provenance ATS | Integration (~Feb 5 go-live) | P0 | Clare Hove, Shawn Gao | BitGo sole signatory; iFrame; Futu/Moomoo sub-clients; Feb 16 client list deadline |
| Haven (Heaven) | Canton USDCX/CBTC collateral + lending | In progress | P0 | Abhishek | ~$3.5B assets at 100% vol; deposit support needed |
| Concrete | DeFi vault (first) | End of Feb | P0 | Emerick | ~50% tech access fee; 9–10 clients (mostly USD1); risk rating TBD |
| Aave | Direct protocol + native BTC borrowing | MOU announced | P1 | Emerick | No exclusivity constraints; DeFi marketplace listing |
| DTCC / Equitable / DUCA | Canton onboarding | In progress | P1 | Abhishek/Canton team | DTCC treasuries; DVP transfers; on-chain settlement |
| Binance | Staking; OES | Testing | P1 | Kevin Son | ~$175M pipeline (~$145M new); 7-day unbonding HYPE pending; flat 10% ownership concern |
| Franklin Templeton | Staking fund (9 coins; ~$15M AUM) | In progress | P1 | Richard | Selected Blockdaemon (validator) + BitGo (custodian); push FT to use Go validators; 7/9 coins supported (HYPE + TRON need work) |
| Kingsway | ~1M locked TON staking | Urgent | P0 | Gaurav/Richard | ~1-week window (Feb context) |
| X Money Group (XMG) | Integration | In progress | P1 | TBD | ~$200K integration fee + upside; push Go validator |
| 21.co | ~$10M ETP | In progress | P1 | Anantha | White-label validator per client |
| P2P SSV | ETH staking via Go validator | Near testing | P1 | Richard | ~$600K integration fee paid by P2P; Alverton initial ~$4M |
| Ton Whales | TON staking | Testing | P2 | Richard | Alongside P2P SSV |
| Midnight Foundation | Privacy chain ($3.3M/3yr) | Commercial | P1 | TBD | $450K NRE; ~$685K/yr recurring; Monument Bank (UK) potential; MPC requirement |

## Major Opportunities / Pipeline

| Opportunity | Stage | Notes |
|-------------|-------|-------|
| Bullish exchange (DeFi skunkworks) | Early discovery | Exchange-side skunkworks (separate from Bullish capital arm which uses Fortify/Firebox). Engineering + corp ops due diligence. Want Eth+Solana DeFi capability, dirty fund checks, pre-tx screening. Interested in **Narval path** (wallet connectivity). Blockaid intro arranged by Akshay. May want to deploy own EVM DeFi protocol — major enterprise win if it materializes. Slack channel agreed for comms. Vince Liu (eng lead), Paul Trudgian (exec sponsor). *(Mar 6, 2026)* |
| Maple Finance | Institutional DeFi | OC charter enables non-fiduciary actions + liquid pools; quantify business impact. Also a Narval launch DApp. |
| Morpho | Institutional DeFi | Vaults marketplace candidate |
| Narval | Institutional DeFi | **Launching this month (Mar 2026)**; qualified custody DeFi access; human-readable tx decoding; DDQ/whitelist DApp process; first DApps: Maro, Maple Finance, Spark; whitelist specific pools OR entire DApp; UI + API access; transactions signed in Narval trusted environment |
| Canton long-term | Tokenized US Treasuries / DTCC settlement | 1–3 year horizon; ~5% of tx fees + SV Cantoncoin rewards |
| Monument Bank (UK) | Midnight / privacy chain custody | ~$10B tokenized fund potential |
| Story Protocol | Go validator | ~$3M Story; spinning up Go validator |

## Key Deal Structures

- **Figure ATS**: Commit/uncommit message flows (not standard withdrawals) require BitGo signatures; REST API for trade reconciliation; FIX for order management; daily ~15-min maintenance window; cloud interconnect (AWS/GCP)
- **Canton SV**: CIP-0074; weight-5 SV; Cantoncoin rewards; milestone-based vesting (custody enablement, Canton token standard, Canton-native asset custody, client adoption); ~$1.16 Cantoncoin; ~$28M/yr at Year 3 (70% treasury lock)
- **Auto Staking commercial model**: Client guarantee = instant withdrawals + daily rewards; BitGo funds liquidity despite bonding/unbonding; infra costs (nodes/validators/monitoring) + capital cost of liquidity buffer = main cost drivers
- **AUC receipt tokens**: Plan to count receipt tokens as AUC (1:1 redeemable IOU via legal agreements)

## Competitive Context

- Blockdaemon + Figment: main validator competitors; build validator compare matrix (deficits, parity plan, single-vendor selling point)
- Coinbase: Agentic Wallets product; Miston Labs moved ~$750M Sooie there
- Circle CPN, Fireblocks, Anchorage: custody/institutional DeFi competitors
- **Blockaid** (pre-tx simulation provider): EVM integration already live at BitGo; Solana support ~weeks away. Forks blockchain, executes tx, shows end state + ML fraud scan. CEO-endorsed security initiative. PM/ENG owner TBD.

## Notable Watch Items

- Vechain: still owes ~25M tokens (~$250K) to seed validator; Stargate NFTs
- Miston Labs: moving ~$750M Sooie to Coinbase; still pursuing other vault opportunities
- Privacy coins: compliance flagged shielded coins as likely hard-no unless auditors/regulators/OC have transparency access
- Insurance/slashing protection: working with Jody + external insurance partners; client FAQ

---

*Last updated: 2026-03-06*
