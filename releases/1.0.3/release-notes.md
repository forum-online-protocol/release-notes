# Forum 1.0.3 Technical Release Notes

## Current Release

**Version:** `1.0.3 (build 6)`  
**Branch:** `v2`  
**Network:** `Sepolia`  
**Prepared:** `2026-03-10`

### Summary

This release moves Forum from a passport-and-wallet prototype into a usable end-to-end social and initiative product. Users can now publish posts and initiatives, discuss them in threads, like content, and manage profiles more comfortably.

### Major Additions

#### Post And Initiative Publishing

- Finalized user post and initiative submission flow from mobile to backend moderation and on-chain publication.
- Added moderation-aware publishing pipeline so content does not appear publicly before approval.
- Hidden pending posts from public timelines.
- Added safety-policy consent gate before publishing.

#### Comments, Threads, And Likes

- Added signed comments flow.
- Improved threaded discussion experience in post detail screens.
- Fixed comment counters and reply count consistency across feed and detail views.
- Polished post interaction surfaces for likes and related actions.
- Social feed now operates as a fuller product surface: posts, likes, comments, repost-oriented feed behavior, and initiative discussion.

#### Profiles And Settings

- Improved profile, public profile, and edit-profile flows.
- Added/expanded profile metadata handling on server and public profile reads.
- Stabilized settings and auth flows.
- Improved profile navigation behavior and screen consistency.

### Voting And On-Chain Flow

- Improved initiative voting UX and state handling in mobile.
- Hardened the canonical initiative vote pipeline on the server.
- Improved batched initiative vote publication reliability and receipt verification flow.
- Extended the underlying vote-publication infrastructure for safer per-initiative operation.
- Continued alignment of mobile, backend, and Sepolia deploy/runtime configuration for real on-chain flow.

### UI / UX Polish

- Large feed and post-detail polish pass, including new feed-card treatment and clearer content hierarchy.
- Better posting loaders and submission feedback.
- Fixed Android back behavior.
- Improved blockchain detail visibility and transaction log surfacing.
- Continued localization cleanup and copy consistency.
- General navigation, layout, and state polish across feed, profile, voting, and settings.

### Platform And Security Improvements

- Continued EIP-712 and nonce/deadline hardening in signed flows.
- Improved eligibility and server-side vote verification alignment.
- Added safer production/dev controls around passport auto-issue and deployment defaults.
- Kept `Demo Mode` and version-check flows available for review/testing and store delivery.

### Future-Ready Foundations

- Prepared runway for a full biometric flow in `v2`, including contract support for biometric commitments and backend feature-flagged stubs.
- Advanced the biometric architecture and implementation groundwork so enrollment and signing flows can be completed in a later release.
- Prepared public node / public RPC groundwork for a more open infrastructure model and future independent operator setup.

### Easy-To-Forget Items Included In This Release

- Hardened batched vote publication and receipt verification flow.
- Moderation gating for pending submissions.
- Transaction log and blockchain detail screens.
- Auth/settings stabilization work.
- Localization cleanup across mobile flows.
- Biometric runway groundwork.
- Public node / public RPC groundwork.

### Release Scope Snapshot

- `User publishing + moderation`
- `Comments / threads`
- `Likes and social interactions`
- `Profile editing and settings`
- `Voting flow hardening`
- `UI / UX polish`
- `Biometric runway preparation`
- `Public node groundwork`
- `Sepolia full on-chain flow hardening`

### Notes

- This release note is based on the current codebase state and the latest `v2` commits, not the older archived localization-only note that previously lived in this file.
- The app remains oriented around `Sepolia` runtime and operator-managed backend flows.
