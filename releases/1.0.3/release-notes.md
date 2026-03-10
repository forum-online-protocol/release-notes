# Forum 1.0.3 Technical Release Notes

**Version:** `1.0.3 (build 6)`  
**Branch:** `v2`  
**Network:** `Sepolia`  
**Prepared:** `2026-03-10`

## Summary

This release moves Forum from a passport-and-wallet prototype into a usable end-to-end social and proposal product. Users can now publish posts and proposals, discuss them in threads, like content, manage profiles more comfortably, and participate in proposal-linked lottery mechanics.

## Major Additions

### Lottery

- Added proposal-linked `ETH` lottery flow.
- Added lottery deployment and lifecycle operations through `ProposalLotteryFactory`.
- Added operator flows for funding, draw, claim, recover-unawarded funds, and sweep-unclaimed funds.
- Added lottery status visibility in feed, post detail, and backend flows.

### Post And Proposal Publishing

- Finalized user post and proposal submission flow from mobile to backend moderation and on-chain publication.
- Added moderation-aware publishing pipeline so content does not appear publicly before approval.
- Hidden pending posts from public timelines.
- Added safety-policy consent gate before publishing.

### Comments, Threads, And Likes

- Added signed comments flow.
- Improved threaded discussion experience in post detail screens.
- Fixed comment counters and reply count consistency across feed and detail views.
- Polished post interaction surfaces for likes and related actions.
- Social feed now operates as a fuller product surface: posts, likes, comments, repost-oriented feed behavior, and proposal discussion.

### Profiles And Settings

- Improved profile, public profile, and edit-profile flows.
- Added and expanded profile metadata handling on server and public profile reads.
- Stabilized settings and auth flows.
- Improved profile navigation behavior and screen consistency.

## Voting And On-Chain Flow

- Improved proposal voting UX and state handling in mobile.
- Hardened the canonical proposal vote pipeline on the server.
- Improved batched proposal vote publication reliability and receipt verification flow.
- Extended the underlying vote-publication infrastructure for safer per-proposal operation.
- Continued alignment of mobile, backend, and Sepolia deploy/runtime configuration for real on-chain flow.

## UI And UX Polish

- Large feed and post-detail polish pass, including new feed-card treatment and clearer content hierarchy.
- Better posting loaders and submission feedback.
- Fixed Android back behavior.
- Improved blockchain detail visibility and transaction log surfacing.
- Continued localization cleanup and copy consistency.
- General navigation, layout, and state polish across feed, profile, voting, and settings.

## Platform And Security Improvements

- Continued EIP-712 and nonce/deadline hardening in signed flows.
- Improved eligibility and server-side vote verification alignment.
- Added safer production and development controls around passport auto-issue and deployment defaults.
- Kept `Demo Mode` and version-check flows available for review, testing, and store delivery.

## Future-Ready Foundations

- Prepared runway for a full biometric flow in `v2`, including contract support for biometric commitments and backend feature-flagged stubs.
- Advanced the biometric architecture and implementation groundwork so enrollment and signing flows can be completed in a later release.
- Prepared public node and public RPC groundwork for a more open infrastructure model and future independent operator setup.

## Scope Snapshot

- `Lottery v1 (ETH)`
- `User publishing + moderation`
- `Comments / threads`
- `Likes and social interactions`
- `Profile editing and settings`
- `Voting flow hardening`
- `UI / UX polish`
- `Biometric runway preparation`
- `Public node groundwork`
- `Sepolia full on-chain flow hardening`
