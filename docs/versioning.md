# How we version and organise these updates

Three things are versioned separately, because they ship on different clocks.

## 1. The platform: calendar versions

The web platform and the services behind it ship continuously. Grouping that into
semantic versions would be false precision, so we use calendar versions instead.

```
2026.09   <- the September 2026 platform release
   |  |
   |  +-- month
   +----- year
```

One calendar version per month. Everything that reached production in that month belongs to it,
and the monthly update file is its release note.

## 2. The apps: semantic versions

Apps are shipped through app stores, so they carry real version numbers that users can see.

| App | Current | Scheme |
|---|---|---|
| Volve Vision mobile | 1.2 | `MAJOR.MINOR`, store builds counted separately |
| VolveMenu | 1.0 | `MAJOR.MINOR`, store builds counted separately |

`MAJOR` changes when the shape of the product changes. `MINOR` changes when features are added.
Build numbers increment on every submission and are not meaningful outside the store.

## 3. The catalogue: not versioned

The camera catalogue changes every day as cameras are added, go offline, recover or are retired.
It is measured, not versioned. Current scale is on the [front page](../README.md#the-catalogue-today).

---

## Where everything lives

```
.
├── README.md                 Entry point: products, scale, direction
├── CHANGELOG.md              Every platform release, newest first
├── ROADMAP.md                Now / Next / Later
├── SECURITY.md               How to report a vulnerability
│
├── products/                 One file per product, full history
│   ├── web-platform.md
│   ├── mobile-apps.md
│   ├── volvemenu.md
│   ├── video-analytics.md
│   ├── operations-console.md
│   └── brand.md
│
├── updates/                  One file per month, the detailed record
│   ├── 2026/2026-09.md ... 2026-02.md
│   ├── 2025/2025-q4.md
│   └── 2022/2022-2023.md
│
├── docs/
│   ├── versioning.md         This file
│   └── what-we-publish.md    Our disclosure policy
│
└── assets/diagrams/          Diagrams, light and dark variants
```

## The format of a monthly update

Every monthly file follows the same shape, so they can be compared at a glance:

1. **In one line** - what the month was about.
2. **Highlights** - the two or three things that mattered.
3. **By product** - what changed, grouped under the six categories below.
4. **Numbers** - catalogue scale at the end of the month, where it moved.

We use the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) categories, with one addition:

| Category | Meaning |
|---|---|
| `Added` | New capability that was not there before |
| `Changed` | Existing behaviour works differently now |
| `Fixed` | Something was broken and now is not |
| `Removed` | A capability was taken out |
| `Performance` | Same behaviour, measurably faster or lighter |
| `Reliability` | Same behaviour, fails less often |

Security work is reported in aggregate only, and only after it has shipped. The reasoning is in
[what we publish](what-we-publish.md).

Dates are ISO 8601 (`YYYY-MM-DD`). Newest entries come first, everywhere.
