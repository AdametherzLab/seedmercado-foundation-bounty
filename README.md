# SeedMercado Foundation Bounty

> ## ⚠️ Real SEED contract address
>
> The **ONLY** legitimate SEED token is [`0xA0FbF7303e37f75F54352d80ae720aEb410777c8`](https://basescan.org/address/0xA0FbF7303e37f75F54352d80ae720aEb410777c8) on Base.
>
> At least one copycat token using the SeedMercado name and logo has been deployed by a third party. It is **not us**. Do not buy, swap, or interact with any SEED token at a different contract address. If you received SEED from the Foundation Bounty, verify the `token` field in the BaseScan tx matches the address above.

**SEED-denominated community contribution program for [SeedMercado](https://seedmercado.io), the heirloom-seed marketplace on Base.**

Community contributors who find bugs, grow the audience, create content, or build features get paid in SEED (the platform's reward token) from a public Foundation Bounty pot. No cash. No gatekeepers. Contributors who believe in the project's direction trade their time for SEED and share the upside.

---

## Pot

| Item | Value |
|---|---|
| Pot wallet | [`seedmercado.base.eth`](https://basescan.org/address/0x19751730b8f5103013aC29C4DdF908b7CF1d90bD) (`0x19751730b8f5103013aC29C4DdF908b7CF1d90bD`) |
| Initial allocation | 50,000 SEED (5% of current supply) |
| Funded | 2026-04-21 ([tx](https://basescan.org/tx/0xfda184a603da01849cf7af96f72b2e5d1b89ec579327a4cc1bb26f6904038984)) |
| Live balance | [See on BaseScan](https://basescan.org/token/0xA0FbF7303e37f75F54352d80ae720aEb410777c8?a=0x19751730b8f5103013aC29C4DdF908b7CF1d90bD) |
| SEED token | [`0xA0FbF7303e37f75F54352d80ae720aEb410777c8`](https://basescan.org/address/0xA0FbF7303e37f75F54352d80ae720aEb410777c8) |

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
| Growth quest: light | follow @seedmercado, claim a free listing, list a seed pack | 1 to 25 SEED (often auto-paid on-platform) |
| Growth quest: heavy | bring 10 verified new users who each claim a listing | 500 SEED |
| Dev: small | merged PR, small UI improvement | 100 to 500 SEED |
| Dev: large | major contract or backend feature PR | 1,000 to 5,000 SEED |

Rewards are nominal SEED amounts. See transparency section below.

---

## Open bounties

Bounties are hosted on external platforms so contributors can discover them through their usual channels. Every listing links back here for the canonical rules.

| Platform | Bounty | Status |
|---|---|---|
| Layer3 | Follow + claim Balcony Bounty #1 (5 SEED) | _posting soon_ |
| Layer3 | List a seed pack (25 SEED) | _posting soon_ |
| Dework | Bug-report intake (50 to 500 SEED by severity) | _posting soon_ |
| Dework | Fix `NOTIFICATION_EMAIL_REQUIRED` frontend modal (500 SEED) | _posting soon_ |
| Bountycaster | Share your SeedMercado garden or review (30 SEED x 5 slots) | _posting soon_ |
| x402 Bazaar | Programmatic bounty intake for autonomous agents | _posting soon_ |

This table updates as listings go live. Submitting on the platform and completing its verification is usually the fastest path. For bounties without platform-native verification, use the Telegram bot below.

---

## How to claim

### Path 1: Platform-native (fastest for quest-style bounties)

Layer3, Bountycaster, and Gitcoin verify claim completion on their own side and trigger the SEED payout automatically. Complete the quest, and your SEED arrives without any additional submission.

### Path 2: Telegram bot (for bug reports, content, custom bounties)

1. Open Telegram and DM [`@SeedMercadoFoundation_bot`](https://t.me/SeedMercadoFoundation_bot)
2. Send `/start`. If this is your first time, the bot will say "invite-only" and the admin will get a notification to whitelist you. Ping `@adamether` on Telegram or X with a short introduction of what you want to contribute and your Base wallet address.
3. Once whitelisted, submit:
   - `/post <tweet-or-cast-URL>` for a content claim (20 SEED)
   - `/milestone <description + evidence>` for a follower-growth or larger claim (500 SEED)
   - Bug reports: see below
4. Admin reviews + approves. SEED lands in your wallet.
5. `/status` shows your claim history at any time.

### Path 3: Bug reports

For bug reports, open a Dework task in the SeedMercado workspace with:
- Steps to reproduce
- Expected vs actual behaviour
- Severity (low, medium, high, critical) + rationale
- Screenshot or console output if relevant

Admin will triage within 48 hours and set the final reward based on the rate card. Critical bugs (fund loss, contract bugs) get direct fast-track attention: email [adametherzlab@gmail.com](mailto:adametherzlab@gmail.com) or DM `@adamether` with subject "CRITICAL BUG".

---

## Transparency (read this before accepting)

**SEED has no DEX price yet.** It is the reward token of the SeedMercado marketplace, earned by users who list seeds, buy seeds, or leave reviews. DEX liquidity is on the Phase 3 roadmap (2,000+ users). Today, SEED has implied value only.

**You are betting on the project.** By accepting SEED as compensation, you are taking an equity-style position in SeedMercado's success. If the marketplace grows and SEED gains liquidity, your SEED is worth something. If it does not, your SEED is a souvenir. The founder accepts the same risk on the same terms.

**This is not employment.** There is no retainer guarantee, no hourly rate, no W-2. Bounties are per-task, payable in SEED only, paid when verified. No invoice, no contract beyond the bounty-by-bounty scope on each platform.

**Cash is not on the table.** The project has no USDC / USDT / stablecoin budget, now or on future engagements. Candidates who counter-offer stablecoin compensation are politely declined. This is not a negotiation stance; it is the structural reality of a founder-stage project that chose equity-style bootstrapping.

---

## Ownership and governance

- **Pot control:** today, `seedmercado.base.eth` is controlled by Adam Etherzlab's phone wallet. A dedicated hot wallet on the VPS signs automated small payouts (capped at ~1,000 SEED rolling balance; compromise radius is 0.1% of supply).
- **Approvals:** every claim is reviewed by the admin. Progressive trust: after a contributor has 3+ cleanly paid claims, small future claims may auto-pay within a 1-hour veto window.
- **Refill:** when the hot wallet drops below 200 SEED, admin tops it up from the cold pot. Pot refills from treasury require a separate, documented decision.
- **Transparency:** every payout is visible on BaseScan. Every claim is recorded in the bot's local store + audit log.

---

## Resources

- [SeedMercado.io](https://seedmercado.io) — the marketplace itself
- [@seedmercado on X](https://x.com/seedmercado) — announcements
- [Balcony Bounty #1](https://seedmercado.io/marketplace/listings/1) — live free-seed listing (first 25 claimers get a FoundingMember1 NFT)
- [SeedMercado contracts](https://basescan.org/address/0xcb3336d980ab6678f68BDd081e2F4D29E0C4CF43) on BaseScan
