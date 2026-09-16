# Changelog

Every platform release, newest first. Follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
with two added categories, `Performance` and `Reliability`. Versioning is explained in
[docs/versioning.md](docs/versioning.md).

Apps carry their own version numbers and are listed under the release they shipped in.

---

## [2026.09] - September 2026
*Mobile app 1.2, in internal testing and not yet released to the stores*

### Added
- Account security centre on the website, the mobile app and the VolveMenu management app: active
  sessions, recent security events, remote sign-out that takes effect everywhere.
- Verification with two further regional search engines.
- 3D version of the brand mascot, usable across products.

### Changed
- Sign in with Apple follows Apple's presentation rules exactly.
- A revoked session now signs every client out cleanly.
- VolveMenu screens on a wall are never signed out by accident.

### Fixed
- Accented characters in camera and place names are normalised rather than deleted.
- A missing camera responds identically in all four languages.
- The map no longer moves a camera behind the bottom sheet.

### Reliability
- An unhealthy camera source is isolated instead of being read as hundreds of dead cameras.
  Several hundred cameras switched off by that fault were recovered.
- Camera health checks rotate through the catalogue nightly.

### Performance
- Repeated browser permission checks cached, removing a network round trip from many calls.

[Full detail](updates/2026/2026-09.md)

---

## [2026.08] - August 2026
*Mobile app 1.1, VolveMenu 1.0*

### Added
- **VolveMenu**, complete: venues, menus, screen pairing, offline delivery, real-time
  updates, media handling, push notifications on iOS, snapshots, share links, demo content.
- German as a fourth full language across site, apps, email, notifications and content.
- Rebuilt map in the mobile app: category filters, camera list, preview markers, directions.
- Full-screen landscape multi-camera view in the mobile app.
- Install banner for phone visitors on the website.

### Changed
- An offline camera keeps its page for a defined window instead of disappearing.
- Pages are offered to search engines only in languages they have real content in.

### Fixed
- Descriptions that were being cut mid-sentence.
- City pages that had been orphaned from their country.

### Performance
- Long camera grids in the app scroll smoothly on older devices.

[Full detail](updates/2026/2026-08.md)

---

## [2026.07] - July 2026
*Mobile app 1.0*

### Added
- **Mobile apps for iOS and Android**: catalogue, player, map, search, favourites, news, profile,
  three languages, themes, widgets, quick actions, voice shortcuts, picture-in-picture, offline
  saved cameras, cameras near you, camera submission, owner analytics, haptics, large-text support.
- Sign in with Apple on iOS and Google sign-in, and in-app account deletion.
- Live viewer counts and live reactions on camera pages.
- Camera reporting for viewers.
- First-party promotional slots on the website.

### Changed
- Advertising layout no longer shifts content while a page settles.

### Performance
- Home and camera pages: less layout movement, faster first paint.

### Reliability
- Backup scheduling moved off a contended hour, with catch-up after a restart.

[Full detail](updates/2026/2026-07.md)

---

## [2026.06] - June 2026

### Added
- News and editorial section: categories, topics, authors, multi-language articles, related cameras.
- Comment moderation across all supported languages.
- Content production pipeline with per-language readiness, covering the whole catalogue.
- Location pages for cities and regions that had none.
- Editorial and bulk content tooling in the operations console.

### Changed
- How camera pages describe themselves to search engines, in every language.
- Country and region naming unified across the catalogue.

### Fixed
- Breadcrumb trails that could point at pages which did not exist.

### Security
- Additional browser-level protections across public surfaces, introduced in a monitoring mode first.

[Full detail](updates/2026/2026-06.md)

---

## [2026.05] - May 2026

### Added
- Accounts: durable sessions, device awareness, sign-up abuse protection.
- Subscriptions and payments: trials, proration, receipts, yearly and per-camera plans.
- Monetisation for camera owners: promoted placement, campaigns, moderation, reporting.
- Owner analytics.
- Recommendations and nearby-camera discovery.
- Operations console with role-based access.
- Automated daily backups with a release-blocking health check.
- Automated release pipelines with manual approval.
- Spanish as a third language.

### Performance
- Caching and database work across the busiest paths.

### Reliability
- Protection against slow or failing upstream camera sources.

[Full detail](updates/2026/2026-05.md)

---

## [2026.04] - April 2026

### Added
- **The new volvevision.com**: catalogue, maps, search, camera, city and country pages, multi-language
  from day one. Replaced the previous generation entirely.
- Automated camera health checking.
- Intake pipeline for new camera sources.
- Automatic submission of new pages to search engines.
- Comments and notifications.

[Full detail](updates/2026/2026-04.md)

---

## [2026.03] - March 2026

### Added
- Recording and archive handling.
- Notification delivery.
- First public landing page.

[Full detail](updates/2026/2026-03.md)

---

## [2026.02] - February 2026

### Added
- The service layer the platform still runs on: cameras, profiles, accounts.
- Payment handling.
- Transactional email.

[Full detail](updates/2026/2026-02.md)

---

## Before the rebuild

- [Q4 2025](updates/2025/2025-q4.md) - the decision to rebuild rather than extend.
- [2022 to 2023](updates/2022/2022-2023.md) - the first generation, no longer in service.
