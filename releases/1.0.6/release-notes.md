# Forum 1.0.6 Technical Release Notes

## Current Release

**Version:** `1.0.6`
**Branch:** `v2`
**Network:** `Sepolia`
**Initial Release:** `2026-04-05`  
**Updated:** `2026-04-15`  
**Addendum Window:** `2026-04-01` - `2026-04-15`

### Summary

Forum `1.0.6` started as a social feature release and was expanded with a stabilization addendum: smart following notifications, profile/feed consistency improvements, legacy content compatibility, better voting metrics, and multiple mobile reliability fixes.

### Major Additions

#### Follow System

- Users can follow and unfollow accounts.
- Follow activity feeds allow tracking updates from followed users.
- On-chain follow system contract integration via `FOLLOW_SYSTEM_ADDRESS`.

#### Threaded Comments

- Comments now support replies, enabling structured threaded discussions.
- Improved comment navigation and reply count consistency.

#### Hashtags And Search

- Posts can include hashtags for content categorization.
- Search by hashtag tags for easier content discovery.

#### Following Push Notifications (Addendum)

- Added signed API path and server worker pipeline for following-post notifications.
- Added smart delivery logic (send-now / digest style behavior) to reduce noisy push patterns.
- Added mobile settings controls for following-post push notifications.

### Enhancements

#### Improved Auto Translation

- More accurate and natural translations across supported languages.
- Server-side translation flow with DeepL integration.
- Reduced duplicate translation requests and improved caching.
- Translation toggle UI unified across posts and profiles.
- Removed on-device translation modules on Android/iOS app layer to reduce runtime complexity.

#### Enhanced On-Chain Vote Details

- Better visibility into blockchain data for each vote.
- Verification insights and transparency improvements.
- Profile verification badge sourcing improvements.

#### Platform Metrics And Stats (Addendum)

- Added `registeredUsers` coverage in public stats endpoints.
- Fixed unique voter count logic to use vote index keys only.

### Performance And Stability

- Performance optimizations for faster feed loading and smoother navigation.
- General bug fixes and stability improvements.
- Server rate limit adjustments for improved throughput.
- Fixed post-NFC crash path caused by undefined module require in mobile flow.
- Applied broader safe-area handling across core screens.
- Fixed iOS feed bottom gap and improved card header layout behavior on small screens.
- Improved legacy author profile/feed resolution for visibility and verified state.

### Profile And Following UX (Addendum)

- Added signed `my-posts` endpoint integration in mobile profile flow.
- Improved follow-state clarity with explicit labels.
- Added unfollow confirmation for safer follow graph actions.
- Improved profile verification/real-name indicator consistency.

### Mobile Delivery Readiness

- Added Android Play Store version automation in CI (`versionCode`/`versionName` override support).
- Aligned in-app version label behavior with server version metadata.

### Localized Release Notes

#### English (Short)

- Improved auto translation
- Follow accounts
- Threaded comments
- Hashtags and search
- Enhanced on-chain vote details
- Smart following notifications
- Better legacy profile/feed compatibility
- Performance improvements and bug fixes

#### Russian (Short)

- Улучшен автоперевод
- Подписка на аккаунты
- Треды в комментариях
- Хэштеги и поиск
- Улучшены детали голосов в блокчейне
- Добавлены push-уведомления по подпискам
- Улучшена совместимость легаси профилей/ленты
- Оптимизация и исправления

#### Apple-Style (English)

- Follow users and stay updated
- Reply to comments with threaded discussions
- Discover content via hashtags
- Improved translations
- Enhanced on-chain vote transparency
- Smart following-feed notifications
- Performance improvements and bug fixes

#### Apple-Style (Russian)

- Подписывайтесь на пользователей
- Отвечайте на комментарии (треды)
- Используйте хэштеги для поиска
- Улучшен автоперевод
- Повышена прозрачность голосов в блокчейне
- Умные уведомления о новых постах в подписках
- Оптимизация и исправления

#### Web3 Pitch (English)

We're making governance more transparent, social, and accessible.

- Follow participants and track their activity
- Engage in structured discussions with threaded replies
- Discover topics through hashtags and search
- Improved multilingual experience with enhanced auto translation
- Deeper on-chain vote insights for full transparency
- Smart notifications for followed authors
- Better legacy profile/feed consistency
- Faster, smoother, and more reliable performance

#### Web3 Pitch (Russian)

Мы делаем управление более прозрачным, социальным и доступным.

- Подписывайтесь на участников и отслеживайте их активность
- Ведите структурированные обсуждения через треды
- Находите темы через хэштеги и поиск
- Улучшенный мультиязычный опыт благодаря автопереводу
- Более глубокая прозрачность голосов через on-chain данные
- Умные уведомления по постам из подписок
- Улучшенная совместимость легаси профилей/ленты
- Быстрая и стабильная работа приложения

### Release Scope Snapshot

- `Follow system`
- `Threaded comments`
- `Hashtags and search`
- `Improved auto translation`
- `Enhanced on-chain vote details`
- `Following push notifications`
- `Profile/follow-state clarity improvements`
- `Legacy profile/feed compatibility`
- `Public stats correctness updates`
- `Performance optimizations`
- `Bug fixes and stability`

### Notes

- The app remains oriented around `Sepolia` runtime and operator-managed backend flows.
