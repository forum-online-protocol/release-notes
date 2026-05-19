# Forum 1.1.0 Technical Release Notes

## Current Release

**Version:** `1.1.0`  
**Branch:** `v2`  
**Network:** `Sepolia` + Dual Network pre-mainnet readiness  
**Prepared:** `2026-05-19`  
**Release Window:** `2026-04-16` - `2026-05-19`

### Summary

Forum `1.1.0` introduces Wallet V2, Lottery, and Dual Network pre-mainnet mode. It also improves the app around the flows users touch most: feed discovery, wallet backup and recovery, wallet sending, voting, search, profiles, NFC passport scanning, and older-account compatibility.

### New Features

#### Wallet V2

- Introduced Wallet V2 as a new wallet foundation for Forum accounts.
- Added a guided upgrade path for existing Wallet V1 users.
- Added passkey-first wallet access preparation.
- Added stronger backup handling before sensitive wallet actions.
- Added encrypted QR wallet transfer and recovery for moving a wallet to another device.
- Added wallet private key export support.
- Kept Wallet V1 fallback available for users who still need it during transition.

#### Wallet Tools

- Added QR scanning for recipient wallet addresses.
- Added gas estimates before wallet sends.
- Made wallet network selection clearer and less mixed with normal wallet actions.
- Moved fallback, export, and recovery tools into Settings.

#### Lottery

- Introduced Lottery as a new Forum product surface.
- Connected Lottery behavior to participation and voting flows.
- Added a simpler instant fixed-payout reward model.
- Added controlled visibility for the intended rollout groups.

#### Dual Network Mode

- Introduced Dual Network mode for the pre-mainnet stage.
- Added controlled network switching for eligible users.
- Prepared the app for Sepolia and Polygon mainnet readiness without broadly opening mainnet behavior.
- Improved network-aware behavior across wallet, feed, voting, and rollout-controlled features.

#### Smart Feed

- Added Smart Feed ranking improvements for fresher and more relevant discovery.
- Tuned popular feed ranking around recent activity, reactions, and discussion momentum.
- Improved handling of legacy and migrated-account posts in feed and profile views.

#### Voting

- Improved pending initiative voting.
- Improved vote status loading.

#### Search, Links, And Profiles

- Added safer link handling inside posts.
- Improved tapping links in feed and post detail screens.
- Improved search for mixed-script names and visually similar characters.
- Improved follower/profile snapshots so social state is clearer.

### Fixes And Improvements

#### Wallet And Account Fixes

- Fixed Wallet V2 voting after upgrade.
- Fixed historical passport-derived wallet recovery.
- Fixed duplicate Wallet V2 registration after migration.
- Fixed mismatched Wallet V2 seed restore handling.
- Fixed stale Wallet V1 session behavior after Wallet V2 upgrade.
- Fixed local passkey login and backup edge cases.
- Fixed wallet clipboard copy behavior.
- Fixed encrypted QR scanner behavior on iOS.
- Fixed wallet migration modal scrolling on iOS.
- Fixed account sign-in recovery UX.
- Added mixed-wallet quarantine handling for unsafe account states.

#### Feed, Profile, And Social Fixes

- Fixed migrated-wallet follow lookups in feed and user profile.
- Fixed author feeds and `my-posts` indexes for older accounts.
- Fixed legacy author visibility in profile and feed contexts.
- Fixed profile post counters and profile/feed consistency.
- Removed noisy profile tab counts.
- Improved profile metadata and name verification refresh behavior.
- Fixed post menu and profile post actions.

#### Voting And Lottery Fixes

- Fixed lottery reward paid status.
- Fixed lottery visibility and rollout edge cases.
- Fixed pending initiative voting and vote stats loading.
- Fixed vote confirmation modal layout on short screens.
- Preserved vote verification nonce values correctly.

#### Search, Links, And Comment Fixes

- Fixed safer external link opening from posts.
- Fixed post text taps across feed and detail views.
- Fixed search behavior for mixed-script and confusable characters.
- Fixed duplicate comment submission protection.
- Fixed post detail comment layout on small screens.
- Fixed Android keyboard composer behavior in post detail.

#### NFC And Mobile Stability Fixes

- Improved NFC passport scan reliability on Android and iOS.
- Stabilized iOS passport NFC retries.
- Hardened MRZ scanner behavior.
- Improved Android passport scan progress feedback.
- Improved app startup latency.
- Improved profile loading performance.
- Fixed Android 15/16 app bar overlap and status bar behavior.
- Fixed iOS build and release plist issues.
- Added mobile runtime compatibility fixes for plural rules.

### Release Scope Snapshot

- `Wallet V2`
- `Wallet V2 upgrade path`
- `Wallet backup and recovery`
- `Encrypted QR wallet transfer`
- `Wallet QR send and gas estimates`
- `Lottery`
- `Dual Network pre-mainnet mode`
- `Smart Feed`
- `Lottery fixed payout`
- `Voting reliability`
- `Search and link handling`
- `Profile and follow consistency`
- `Legacy account compatibility`
- `NFC passport scan stability`
- `Mobile performance and stability`

### Notes

- Wallet V2 and Identity V2 remain gradually rolled out rather than broadly opened to every user at once.
- This release note focuses on product features and user-visible fixes; internal deployment and infrastructure work is intentionally omitted.
- This release note is based on `v2` commits merged between `2026-04-16` and `2026-05-19`.
