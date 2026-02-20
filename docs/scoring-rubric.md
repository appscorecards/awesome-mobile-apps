# Scoring rubric

Every scorecard in this repo uses a 1–5 integer score on five dimensions.
This rubric is the reference for what those numbers mean.

## Dimensions

### Accuracy
How closely the app's claimed output matches reality when tested.
Interpretation depends on the category: for a nutrition app, this is
calorie and macro fidelity against weighed meals. For a password manager,
this means zero-loss reliability. For a fitness tracker, this is pace and
distance accuracy vs. a known reference.

- **5** — Reference-quality. Errors are below the noise floor of the
  user's ability to measure.
- **4** — Tight. Occasional small errors that don't affect decisions.
- **3** — Usable. Errors are noticeable but acceptable for casual use.
- **2** — Wide. Errors large enough that users should double-check.
- **1** — Unreliable.

### Core utility
How well the app does its core advertised function.

- **5** — Best in category for the advertised workflow.
- **4** — Very good; a small subset of the advertised features is weaker.
- **3** — Does the core job; several advertised features feel shallow.
- **2** — Missing obvious features or has significant workflow gaps.
- **1** — Primary function is unreliable or absent.

### Privacy
Data handling, policy transparency, business model alignment.

- **5** — Open source or audited, no ad network, clear policy, minimal data.
- **4** — Clear policy, no ad network, reasonable data minimization.
- **3** — Policy exists but some ambiguity; subscription-funded.
- **2** — Ad-funded or policy has notable gaps.
- **1** — Evidence of user-hostile data practices.

### Pricing transparency
How clearly the cost structure is communicated up front.

- **5** — All tiers, limits, and price shown before account creation.
- **4** — Clear but requires one extra click to find a specific detail.
- **3** — Limits or price surfaces only after sign-up.
- **2** — Price changes post-onboarding or dark patterns in the upgrade flow.
- **1** — Price is hidden until after significant user investment.

### UX
Interface quality, learnability, daily-use polish.

- **5** — Delightful. Nothing fights you.
- **4** — Smooth. A few minor rough edges.
- **3** — Functional. Visible rough edges but not blocking.
- **2** — Frustrating in the common path.
- **1** — Actively hard to use.

## Composite score

The `overall` field in the front-matter is the arithmetic mean of the
five dimension scores, rounded to one decimal. It exists for quick
scanning but the per-dimension scores are the honest ones — an app with
4-4-5-5-5 (overall 4.6) and an app with 5-5-5-5-3 (overall 4.6) are not
the same recommendation.

## What we do not score

- Popularity, market share, or number of users.
- Celebrity endorsement or media coverage.
- The color of the icon.

## Review cadence

Scorecards are dated with `last_reviewed: YYYY-MM`. If a scorecard is
older than 12 months we either refresh it or add a note that we haven't
re-tested recently.
