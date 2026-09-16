# What we publish, and what we do not

This repository exists so that people following Volve Vision can see real progress without
being given access to anything private. That only works if the line is drawn clearly and held.

## What you will find here

- What shipped, described by what it does for the person using it.
- Which product it belongs to and when it reached production.
- The category of engineering work behind it: performance, reliability, localisation, accessibility.
- Catalogue scale, taken from sources anyone can check.
- Direction of travel, clearly marked as intent rather than commitment.

## What you will not find here

Not because it is secret for its own sake, but because publishing it would help someone attack
the platform and help nobody else:

- Names, addresses or shapes of the services that run the platform.
- Hostnames, endpoints, parameters or payloads of any interface.
- The technology stack, versions, hosting providers or deployment mechanics.
- How authentication, authorisation, rate limiting or abuse protection are implemented.
- Descriptions of specific vulnerabilities, including ones already fixed.
- Anything about internal tooling, scripts, data models or operational runbooks.
- Traffic, revenue, user counts or any other business metric.

## How we handle security work

Security work is real work, and a lot of it happened in 2026. Reporting it honestly without
turning the report into a map for an attacker means following three rules:

1. **Aggregate, never itemise.** We say that account and session handling was hardened. We do not
   say what was wrong, where, or how it was exploited.
2. **Only after it ships.** Nothing is described while a fix is still rolling out.
3. **No timing signals.** We do not publish when reviews happen, what they cover, or what they found.

An independent review of the account security work was carried out in September 2026 and its
findings were addressed. That is the level of detail we are comfortable with, and it is the level
you will see from us.

## Reporting something to us

If you believe you have found a security issue, please follow [SECURITY.md](../SECURITY.md).
We would much rather hear from you privately than read about it anywhere else.

## Corrections

If something here is wrong, inaccurate or out of date, open an issue on this repository and we
will correct it. We would rather be corrected in public than be quietly wrong.
