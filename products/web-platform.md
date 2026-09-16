# Web platform

**[volvevision.com](https://volvevision.com)** - the live camera catalogue, and the account layer
underneath it. Live since April 2026, shipping continuously since.

It is the oldest surface of the current platform and the one every other product leans on: the
catalogue, the content, the accounts and the billing all live here first and reach the apps second.

---

## What it does

- A browsable, searchable catalogue of public cameras in 98 countries, with its own page for every
  camera, city and country.
- Maps, filters and search that work across four languages.
- Accounts: sign in, saved cameras, preferences, notifications, security.
- Camera owners can submit a camera, see how it performs and earn from it.
- Editorial: a news section with its own topics, authors and categories.
- Subscriptions and payments for owners who want more than the free tier.

---

## History

### September 2026

- **Added** an account security centre: every active session, every recent security event, and the
  ability to end a session anywhere, from anywhere.
- **Changed** how missing cameras respond, so that every language behaves identically instead of
  only the default one.
- **Fixed** camera titles and addresses losing accented characters, which had been quietly
  damaging how pages were found.
- **Reliability** improvements to how quickly the catalogue reacts to a camera source misbehaving.

### August 2026

- **Added** German as a fourth full language: the whole site, not a partial translation.
- **Added** an install banner for people arriving on a phone, pointing at the native apps.
- **Changed** how offline cameras are treated, so a camera that goes dark keeps its page and its
  history for a defined window instead of disappearing.
- **Changed** which pages are offered to search engines, so that a page is only offered in a
  language it genuinely has content in.

### July 2026

- **Performance** work across the home page and camera pages: less layout movement while loading,
  faster first paint, lighter pages.
- **Changed** the advertising layout so it stops shifting content while a page settles.
- **Added** first-party promotional slots that behave predictably alongside third-party ones.

### June 2026

- **Added** the news and editorial section, with categories, topics, authors and multi-language
  articles.
- **Added** comment moderation that hides abusive comments automatically across all languages.
- **Added** structured location pages for cities and regions that previously had no home.
- **Changed** how camera pages describe themselves to search engines, across every language.

### May 2026

- **Added** accounts in their modern form: sessions that survive properly, sign-in protection, and
  device-aware session management.
- **Added** subscriptions and payments, including trials, upgrades, receipts and per-camera plans.
- **Added** monetisation for camera owners: promoted placement, campaign management and reporting.
- **Added** owner analytics, so someone publishing a camera can see how it is doing.
- **Added** recommendations and nearby-camera discovery.
- **Reliability** work on how the platform behaves when an upstream camera source is slow or down.

### April 2026

- **Added** the platform itself. The new site went live with the catalogue, maps, search and
  camera pages, replacing the previous generation entirely.
- **Added** the first automated camera health checks.
- **Added** the pipeline that brings in new camera sources and prepares them for publication.

---

Monthly detail, including work that is not visible on the surface:
[updates/](../updates/README.md).
