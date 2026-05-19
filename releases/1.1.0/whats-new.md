# What's New In Forum 1.1.0

**Version:** `1.1.0`  
**Prepared:** `2026-05-19`  
**Release Window:** `2026-04-16` - `2026-05-19`

Forum `1.1.0` introduces two important foundations for the next stage of Forum: Wallet V2 and Dual Network mode. It also adds a smarter feed, better wallet recovery tools, easier wallet sending, and fixes for older account, profile, voting, search, and NFC flows.

These new features will roll out gradually through cohorts. Some users may see Wallet V2 or Dual Network mode earlier than others while the rollout is checked and expanded.

## Highlights

### Introducing Wallet V2

- Forum now has a new Wallet V2 system.
- Wallet V2 is designed to make account ownership safer, easier to recover, and less tied to fragile old wallet behavior.
- Existing users can be moved into Wallet V2 through a guided upgrade flow.
- Older Wallet V1 access remains available for people who still need it during the transition.
- The app blocks confusing edge cases, like creating a duplicate V2 wallet or restoring the wrong wallet.

### Dual Network Mode

- Forum now has a Dual Network mode for the pre-mainnet stage.
- The app can prepare users and features for both the current test network and the upcoming mainnet path.
- Network switching is controlled through cohorts, so users are not pushed into mainnet behavior before it is ready.
- This gives Forum a safer bridge from Sepolia testing toward Polygon mainnet readiness.

### Smarter Feed

- The feed now does a better job of showing active and relevant posts.
- Popular posts are ranked with more attention to recent activity, reactions, and discussion momentum.
- Fresh posts have a better chance to appear when they start getting attention.
- Legacy and migrated account posts are handled more consistently, so profile and feed views match better.

### Better Wallet Backup And Recovery

- Wallet V2 adds clearer backup and recovery steps.
- You can use encrypted QR transfer to move or recover a wallet on another device.
- Older passport-based wallets can be recovered more reliably.
- Wallet export, fallback, and recovery tools now live in Settings where they are easier to find.

### More Useful Wallet Tools

- Sending from the wallet is easier: scan a recipient QR code instead of pasting an address.
- Gas estimates are shown before sending, so the action is easier to understand.
- Network selection is cleaner and less mixed into everyday wallet actions.
- Copying wallet data and scanning encrypted QR codes is more reliable, especially on iOS.

### Voting Improvements

- Voting on pending initiatives and loading vote status is more reliable.
- Wallet V2 users can vote more reliably after upgrading.
- Vote confirmation screens work better on smaller phones.

### Better Feed, Search, And Profiles

- Links inside posts are easier to tap.
- External links open through a safer path.
- Search works better with names and words that mix similar-looking characters from different alphabets.
- Profile posts, author feeds, and follow information are more consistent for older and migrated accounts.

### Fixes And Reliability

- NFC passport scanning is more stable on Android and iOS.
- App startup and profile loading are faster.
- Older account and profile data is handled more consistently.
- Several wallet copy, scanner, backup, sign-in, and recovery edge cases were fixed.

## In Short

Forum `1.1.0` makes the app feel safer and more complete: Wallet V2 gives Forum a stronger wallet foundation, Dual Network mode prepares the path toward mainnet, the feed is better at surfacing useful posts, and older account, wallet, voting, profile, search, and NFC flows are more reliable.

For technical details, see [release-notes.md](./release-notes.md).
