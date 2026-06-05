---
app: "HealthSync"
category: "fitness"
platforms: ["iOS"]
last_reviewed: "2026-06"
pricing: "Free TestFlight beta"
scores:
  accuracy: 3
  core_utility: 3
  privacy: 4
  pricing_transparency: 3
  ux: 3
overall: 3.2
---

# HealthSync

**Category:** Fitness · **Platforms:** iOS · **Reviewed:** June 2026

HealthSync is a native iOS app for syncing selected Apple Health data from
HealthKit to a private backend API. It is closer to a personal data pipe than a
consumer workout tracker: the useful workflow is exporting steps, heart data,
sleep, workouts, body metrics, and selected nutrition records to an endpoint the
user controls.

## What it does well

- **Private-backend fit.** Users configure their own backend URL and token
  instead of giving a third-party cloud account broad health-data access.
- **Explicit HealthKit scope.** The app is built around selected data types and
  HealthKit permissions rather than a bulk Apple Health export.
- **Useful retry model.** Queued sync and backfill workflows are a better match
  for unreliable mobile networks than one-off CSV export.

## Where it falls short

- **Narrow audience.** This is for users with a backend API or self-hosted
  dashboard, not for people who only want charts in a polished consumer app.
- **Beta distribution.** Access is through TestFlight, so onboarding is less
  direct than a public App Store install.
- **Backend responsibility shifts to the user.** Privacy is strong only if the
  configured destination is operated carefully.

## Score rationale

- **Accuracy (3/5):** HealthKit is the source of truth, but the app's value
  depends on user-selected types, backend ingestion, and sync reliability.
- **Core utility (3/5):** Strong for Apple Health to private API sync; not a
  general fitness tracker.
- **Privacy (4/5):** Data goes to a user-configured endpoint, but the endpoint
  remains outside the app's control.
- **Pricing transparency (3/5):** The current beta is free, but long-term public
  pricing is not yet a normal store listing.
- **UX (3/5):** Focused beta workflow; less polished than mature consumer
  health apps.

## Alternatives

- If you want a social fitness tracker, see [`strava.md`](strava.md).
- If you want detailed nutrition logging, see [`cronometer.md`](cronometer.md).

## Links

- Website: https://healthsync.megabyte.sh/apple-health-app-sync
