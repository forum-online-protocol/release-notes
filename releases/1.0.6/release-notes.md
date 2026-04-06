# Forum 1.0.6 Technical Release Notes

## Current Release

**Version:** `1.0.6`
**Branch:** `v2`
**Network:** `Sepolia`
**Prepared:** `2026-04-05`

### Summary

This release introduces social graph features, threaded discussions, hashtag-based content discovery, improved multilingual support, and deeper on-chain vote transparency.

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

### Enhancements

#### Improved Auto Translation

- More accurate and natural translations across supported languages.
- Server-side translation flow with DeepL integration.
- Reduced duplicate translation requests and improved caching.
- Translation toggle UI unified across posts and profiles.

#### Enhanced On-Chain Vote Details

- Better visibility into blockchain data for each vote.
- Verification insights and transparency improvements.
- Profile verification badge sourcing improvements.

### Performance And Stability

- Performance optimizations for faster feed loading and smoother navigation.
- General bug fixes and stability improvements.
- Server rate limit adjustments for improved throughput.

### Localized Release Notes

#### English (Short)

- Improved auto translation
- Follow accounts
- Threaded comments
- Hashtags and search
- Enhanced on-chain vote details
- Performance improvements and bug fixes

#### Russian (Short)

- Улучшен автоперевод
- Подписка на аккаунты
- Треды в комментариях
- Хэштеги и поиск
- Улучшены детали голосов в блокчейне
- Оптимизация и исправления

#### Apple-Style (English)

- Follow users and stay updated
- Reply to comments with threaded discussions
- Discover content via hashtags
- Improved translations
- Enhanced on-chain vote transparency
- Performance improvements and bug fixes

#### Apple-Style (Russian)

- Подписывайтесь на пользователей
- Отвечайте на комментарии (треды)
- Используйте хэштеги для поиска
- Улучшен автоперевод
- Повышена прозрачность голосов в блокчейне
- Оптимизация и исправления

#### Web3 Pitch (English)

We're making governance more transparent, social, and accessible.

- Follow participants and track their activity
- Engage in structured discussions with threaded replies
- Discover topics through hashtags and search
- Improved multilingual experience with enhanced auto translation
- Deeper on-chain vote insights for full transparency
- Faster, smoother, and more reliable performance

#### Web3 Pitch (Russian)

Мы делаем управление более прозрачным, социальным и доступным.

- Подписывайтесь на участников и отслеживайте их активность
- Ведите структурированные обсуждения через треды
- Находите темы через хэштеги и поиск
- Улучшенный мультиязычный опыт благодаря автопереводу
- Более глубокая прозрачность голосов через on-chain данные
- Быстрая и стабильная работа приложения

### Release Scope Snapshot

- `Follow system`
- `Threaded comments`
- `Hashtags and search`
- `Improved auto translation`
- `Enhanced on-chain vote details`
- `Performance optimizations`
- `Bug fixes and stability`

### Notes

- The app remains oriented around `Sepolia` runtime and operator-managed backend flows.
