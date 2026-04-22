# SeedMercado Foundation Bounty

**LIVE 2026-04-21** — 50,000 SEED funded on-chain at [`seedmercado.base.eth`](https://basescan.org/token/0xA0FbF7303e37f75F54352d80ae720aEb410777c8?a=0x19751730b8f5103013aC29C4DdF908b7CF1d90bD). Pays community contributors in SEED using the Slicing Pie equity model.

**First organic bounty paid 2026-04-22** (claim #2, 20 SEED, real external contributor for a quality retweet).

→ **[Claim a bounty in 60 seconds](#claim-in-60-seconds)** · **[Rate card](#rate-card)** · **[Wallets & transparency](#wallets--transparency)** · **[Open bounties](#open-bounties)**

> ## ⚠️ Real SEED contract address
>
> The **ONLY** legitimate SEED token is [`0xA0FbF7303e37f75F54352d80ae720aEb410777c8`](https://basescan.org/address/0xA0FbF7303e37f75F54352d80ae720aEb410777c8) on Base.
>
> At least one copycat token using the SeedMercado name and logo has been deployed by a third party. It is **not us**. Do not buy, swap, or interact with any SEED token at a different contract address. If you received SEED from the Foundation Bounty, verify the `token` field in the BaseScan tx matches the address above.

**SEED-denominated community contribution program for [SeedMercado](https://seedmercado.io), the heirloom-seed marketplace on Base.**

Community contributors who find bugs, grow the audience, create content, or build features get paid in SEED (the platform's reward token) from a public Foundation Bounty pot. No cash. No gatekeepers. Contributors who believe in the project's direction trade their time for SEED and share the upside.

---

## 3 quick wins

Pick one. Submit. Get paid in SEED.

| Win | Reward | How |
|---|---|---|
| **Tweet or Farcaster cast** about SeedMercado | 20 to 50 SEED | Quote the @seedmercado X or @seedmercado Farcaster intro, tag #BuildOnBase. Submit the URL via the Telegram bot below. |
| **Report a bug** on seedmercado.io | 20 to 5,000 SEED by severity | Open a Bug Bounty issue on this repo. Use the [bug-bounty issue form](https://github.com/AdametherzLab/seedmercado-foundation-bounty/issues/new?template=bug-bounty.yml). |
| **List a real seed pack** on seedmercado.io | 10 SEED + lister bonuses | Go to [SeedMercado.io](https://seedmercado.io), create a listing for a real heirloom seed variety you grew. |

First 10 clean claims get a shoutout on @seedmercado. That's the only promise. Everything else is on the rate card.

---

## Claim in 60 seconds

1. **DM [`@SeedMercadoFoundation_bot`](https://t.me/SeedMercadoFoundation_bot)** on Telegram
2. **Send** `/start 0xYOUR_BASE_WALLET_ADDRESS` — registers you as a contributor and records your payout wallet
3. **Submit proof:**
   - `/post <tweet-or-cast-URL>` for content claims
   - `/milestone <description + evidence>` for growth or larger claims
   - Bug reports: open a GitHub Issue on this repo (link above)
4. **Admin approves** within 24-48 hours. SEED lands in the wallet you registered — usually in under a minute after approval.

You can check your claims anytime with `/status`.

---

## Wallets & transparency

Three project-controlled wallets make up the SEED supply. Every balance and transfer is public on Base.

| Role | Address | Balance (approx) | Purpose |
|---|---|---|---|
| **Treasury** (genesis mint) | [`0xc226...9310`](https://basescan.org/token/0xA0FbF7303e37f75F54352d80ae720aEb410777c8?a=0xc226f2A5d61103EC31672D97aD1a179b64BE9310) | ~950,000 SEED (95% of supply) | Long-term reserve. Rarely touched. Future allocations (liquidity, incentive pools, etc.) will move from here with explicit public announcement before each transfer. |
| **Cold bounty pot** `seedmercado.base.eth` | [`0x1975...90bD`](https://basescan.org/token/0xA0FbF7303e37f75F54352d80ae720aEb410777c8?a=0x19751730b8f5103013aC29C4DdF908b7CF1d90bD) | ~49,000 SEED (Foundation Bounty reserve) | Holds the bounty pool. Signed only by admin's phone wallet, off-VPS. Funds larger/manual payouts and refills the hot wallet. |
| **Hot payout wallet** | [`0x0219...5b87`](https://basescan.org/token/0xA0FbF7303e37f75F54352d80ae720aEb410777c8?a=0x02196a230b9433cB24324f26202A131978A95b87) | ~1,000 SEED (rolling) | Signs small bot-initiated `/payout` transactions for speed. Capped at 1,000 SEED per transaction. Blast radius if VPS is compromised: ~1,000 SEED = 0.1% of supply. |

### How payouts actually flow

- **Small + approved claims (up to 1,000 SEED):** admin approves → bot signs with hot wallet → SEED lands in contributor's wallet in under a minute. No cold-pot movement per claim.
- **Larger payouts** (high-severity bug bounties, large dev bounties): admin signs directly from the cold pot via phone wallet, then records the tx in the bot via `/paid <claim> <tx>` so the audit trail stays complete.

### Hot wallet replenishment rule

When the hot wallet drops below 300 SEED, the bot DMs the admin. Admin manually transfers 1,000 SEED from cold pot to hot wallet from their phone wallet. **The bot does NOT auto-refill itself** — that would defeat the blast-radius cap. Every refill is a deliberate, human-signed, BaseScan-visible transfer.

### On-chain milestones

| Event | Date | Tx |
|---|---|---|
| Pot funded (50k SEED from treasury → cold pot) | 2026-04-21 | [`0xfda1...8984`](https://basescan.org/tx/0xfda184a603da01849cf7af96f72b2e5d1b89ec579327a4cc1bb26f6904038984) |
| First hot wallet refill (1k SEED from cold pot → hot wallet) | 2026-04-21 | [`0x7fad...615f`](https://basescan.org/tx/0x7fad19607188b25a452253cd551b58395845f61fe0e46562221a9defdca3615f) |
| First organic bounty paid (20 SEED to external contributor for a retweet) | 2026-04-22 | see bot audit log + hot wallet's outbound transfers on BaseScan |

---

## Rate card

| Category | Examples | Reward |
|---|---|---|
| Bug: low | typo, broken link, missing alt text | 20 SEED |
| Bug: medium | UX defect, bad error message, display bug | 50 to 100 SEED |
| Bug: high | data-loss risk, bad state, price mis-display | 200 to 500 SEED |
| Bug: critical | fund loss, unauth access, contract bug | 1,000 to 5,000 SEED (case-by-case) |
| Content: short | quality tweet/cast about SeedMercado with real engagement | 20 to 50 SEED |
| Content: long | blog post, TikTok, YouTube review with 500+ real views | 200 to 500 SEED |
| Growth quest: light | follow @seedmercado, claim a free listing, list a seed pack | 1 to 25 SEED |
| Growth quest: heavy | bring 10 verified new users who each claim a listing | 500 SEED |
| Dev: small | merged PR, small UI improvement | 100 to 500 SEED |
| Dev: large | major contract or backend feature PR | 1,000 to 5,000 SEED |

Rewards are nominal SEED amounts. See [transparency](#transparency-read-this-before-accepting) before accepting.

---

## Open bounties

Live channels to discover bounties:

| Channel | Status | Link |
|---|---|---|
| **GitHub Issues** (this repo) | **LIVE** — primary channel | [Issues tagged `bounty:open`](https://github.com/AdametherzLab/seedmercado-foundation-bounty/issues?q=is%3Aopen+is%3Aissue+label%3A%22bounty%3Aopen%22) |
| **Bountycaster** (Farcaster) | **LIVE** | [30 SEED x 5 content bounty](https://farcaster.xyz/seedmercado) |
| **@seedmercado on X** | **LIVE** — posts + mentions | [x.com/seedmercado](https://x.com/seedmercado) |
| **Telegram bot** | **LIVE** | [@SeedMercadoFoundation_bot](https://t.me/SeedMercadoFoundation_bot) |
| Gitcoin bounties | Deferred | — |
| Layer3 quests | Deferred (self-serve flow unclear for small projects) | — |
| Dework tasks | Deferred (Base L2 not supported for on-chain rewards) | — |

### Current open dev bounty

- [#1 Frontend modal for `NOTIFICATION_EMAIL_REQUIRED` error](https://github.com/AdametherzLab/seedmercado-foundation-bounty/issues/1) — **500 SEED**

---

## Transparency (read this before accepting)

**SEED has no DEX price yet.** It is the reward token of the SeedMercado marketplace, earned by users who list seeds, buy seeds, or leave reviews. DEX liquidity is on the Phase 3 roadmap (2,000+ users). Today, SEED has implied value only.

**You are betting on the project.** By accepting SEED as compensation, you are taking an equity-style position in SeedMercado's success. If the marketplace grows and SEED gains liquidity, your SEED is worth something. If it does not, your SEED is a souvenir. The founder accepts the same risk on the same terms.

**This is not employment.** There is no retainer guarantee, no hourly rate, no W-2. Bounties are per-task, payable in SEED only, paid when verified. No invoice, no contract beyond the bounty-by-bounty scope on each platform.

**Cash is not on the table.** The project has no USDC / USDT / stablecoin budget, now or on future engagements. Candidates who counter-offer stablecoin compensation are politely declined. This is not a negotiation stance; it is the structural reality of a founder-stage project that chose equity-style bootstrapping.

---

## Ownership and governance

- **Pot control:** see [Wallets & transparency](#wallets--transparency) above for full breakdown.
- **Approvals:** every claim is reviewed by the admin. Progressive trust: after a contributor has 3+ cleanly paid claims, small future claims may auto-pay within a 1-hour veto window (not yet enabled).
- **Refill:** when hot wallet drops below 300 SEED, bot DMs admin; admin tops up 1,000 SEED from cold pot via phone wallet. Pot refills from treasury require a separate, publicly announced decision.
- **Transparency:** every payout is visible on BaseScan. Every claim is recorded in the bot's local store + audit log.
- **Sybil defense:** contributors who `/start` self-register are admin-review-gated on their first claim. Duplicate claims (same URL) within 30 days are auto-rejected. Daily submission cap per contributor.

---

## Resources

- [SeedMercado.io](https://seedmercado.io) — the marketplace itself
- [@seedmercado on X](https://x.com/seedmercado) — announcements + autonomous reply bot
- [@seedmercado on Farcaster](https://farcaster.xyz/seedmercado) — same brand, crypto-native audience
- [Balcony Bounty #1](https://seedmercado.io/marketplace/listings/1) — live free-seed listing (first 25 claimers get a FoundingMember1 NFT)
- [SeedMercado marketplace contract](https://basescan.org/address/0xcb3336d980ab6678f68BDd081e2F4D29E0C4CF43) on BaseScan
