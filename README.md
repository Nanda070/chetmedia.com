# ChetMedia

### Аниме-платформа от Cheterin Group

[![Сайт](https://img.shields.io/badge/сайт-chetmedia.com-e11d48?style=for-the-badge)](https://chetmedia.com)
[![Discord](https://img.shields.io/badge/Discord-Cheterin%20Group-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/cheterin)
[![Releases](https://img.shields.io/badge/APK-Releases-111827?style=for-the-badge&logo=android&logoColor=white)](https://github.com/Nanda070/chetmedia.com/releases)

**ChetMedia** объединяет каталог аниме, просмотр, личный кабинет и совместный просмотр. Большая часть каталога и плеера доступна без регистрации; аккаунт добавляет синхронизацию прогресса, списки, социальные функции и уведомления.

> **Сайт:** [https://chetmedia.com](https://chetmedia.com)  
> **Это репозиторий:** публичные **APK / Releases**, release notes и project info для ChetMedia.

> **Статус Shorts:** раздел, API, админ-инструменты и генерация Shorts сейчас отключены. Старые записи удалены из production SQLite.

## Android APK / TV (sideload)

Публичные сборки оболочки (телефон / планшет / Android TV) публикуются в **[Releases](https://github.com/Nanda070/chetmedia.com/releases)** этого репозитория.

| | |
| --- | --- |
| Скачать | [Latest Release](https://github.com/Nanda070/chetmedia.com/releases/latest) → файл `.apk` |
| Статус | APK shell в разработке — пока релизов может не быть; placeholder готов |
| Установка | Sideload: разрешить «установку из этого источника» / unknown sources; на TV при необходимости ADB |
| Auto-update | Планируется: shell проверит версию → скачает с Releases → предложит установить; ручной путь через Releases тоже ок |
| Что внутри | Тонкий WebView/shell поверх сайта ChetMedia — не отдельный native rewrite |

**Disclaimer:** sideload вне магазинов — на ваш риск и по правилам вашей платформы. В репозитории нет секретов, keystore и `.env`.

## Возможности

### Каталог и просмотр
- Каталог, поиск, топы, онгоинги, карточки тайтлов и расписание релизов на основе Shikimori/AniLibria данных.
- Плеер с несколькими провайдерами, выбором качества, HLS-проксированием, Cinema Mode и отметками для пропуска опенинга/эндинга.
- Продолжение просмотра: эпизод и позиция сохраняются в профиле и доступны в истории.
- Cloudflare-прокси для публичного сайта и same-origin HLS-маршруты помогают обеспечить доступность для аудитории из РФ.

### Личный кабинет и сообщество
- Регистрация, вход через Discord, публичные профили, подписки и настройки приватности активности.
- Списки «Смотрю», «В планах», «Просмотрено», «Дропнуто», пользовательские категории и импорт списков из Shikimori.
- Уведомления о новых эпизодах по тайтлам из списка и серии дней просмотра.
- «Чредс» — новостная и социальная лента сообщества с реакциями и жалобами.
- Watch Party: комнаты с синхронным воспроизведением, очередью, чатом, реакциями и гостевыми приглашениями.
- Drop Night: запланированный общий старт эпизода с комнатой для просмотра.

### Контент и безопасность
- Отдельная 18+ / hentai-зона с доступом, который администратор выдаёт пользователю.
- Жалобы на комментарии и записи, модерация и аудит администраторских действий.
- Панели администратора и модератора для пользователей, комнат, публикаций, флагов функций, фоновых задач и состояния сервисов.
- Runtime feature flags и rollout для безопасного включения отдельных возможностей; данные каталога и кеши ориентированы на работу на небольшом VPS.

## Быстрый старт

1. Открой [chetmedia.com](https://chetmedia.com), выбери тайтл в [каталоге](https://chetmedia.com/catalog) или на главной.
2. Войди через Discord или зарегистрируйся, чтобы сохранять прогресс, списки и настройки.
3. Для совместного просмотра создай комнату или используй [гостевое приглашение](https://chetmedia.com/room/join).
4. Проверь [расписание](https://chetmedia.com/schedule) и [Чредс](https://chetmedia.com/threads).

## Основные ссылки

| Раздел | Ссылка |
| --- | --- |
| Каталог · Топ · Расписание | [catalog](https://chetmedia.com/catalog) · [top](https://chetmedia.com/top) · [schedule](https://chetmedia.com/schedule) |
| Профиль · Списки · Комнаты | [settings](https://chetmedia.com/settings) · [list](https://chetmedia.com/list) · [room/join](https://chetmedia.com/room/join) |
| Сообщество | [threads](https://chetmedia.com/threads) · [community](https://chetmedia.com/community) · [authors](https://chetmedia.com/authors) |
| Сервис · Правовое | [status](https://chetmedia.com/status) · [terms](https://chetmedia.com/legal/terms) · [privacy](https://chetmedia.com/legal/privacy) · [DMCA](https://chetmedia.com/legal/dmca) |
| APK Releases | [github.com/Nanda070/chetmedia.com/releases](https://github.com/Nanda070/chetmedia.com/releases) |

## Вопросы и поддержка

Вопросы и баги по продукту — в [Discord Cheterin Group](https://discord.gg/cheterin).

## Сообщество и возраст

Общение, новости и поддержка: [discord.gg/cheterin](https://discord.gg/cheterin). Сервис рассчитан на пользователей от 16 лет или возраста цифровой дееспособности в их стране; правила 18+ описаны в [условиях](https://chetmedia.com/legal/terms).

<p align="center"><strong>ChetMedia</strong> · смотри спокойно, делись моментами, заходи в комнату с друзьями.</p>
