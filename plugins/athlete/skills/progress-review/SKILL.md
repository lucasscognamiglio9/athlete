---
name: progress-review
description: Review verified training history and decide what should continue or change next. Use for weekly or block reviews, progress or adherence questions, stagnation analysis, readiness to progress, and evaluating an accepted rule. Questions only about why an existing programming choice was designed belong to training-design.
---

# Progress Review

Convert verified history into the smallest justified next decision.

Read [`../../shared/coach-core.md`](../../shared/coach-core.md) and [`../../shared/canonical-file.md`](../../shared/canonical-file.md) completely before acting. Read [`../../shared/evidence-protocol.md`](../../shared/evidence-protocol.md) when its decision threshold applies.

## 1. Define the review window

Read the active plan version, accepted rules, relevant sessions, and prior decisions. Select the shortest window that can answer the athlete's question while preserving meaningful context.

Continue when the data used, missing data, and comparison basis are explicit.

## 2. Interpret the response

Assess execution and adherence before interpreting progression. Compare observed dose, effort, performance, and consistency with the plan. Separate a single-session fluctuation from a repeated pattern and keep approximate data approximate.

Continue when each conclusion is traceable to canonical observations or clearly marked inference.

## 3. Select one decision path

- **Accepted rule:** apply it only when confirmed data satisfy one active, visible, unambiguous rule.
- **Material change:** recommend it and wait for authorization.
- **Maintain:** keep the current plan when evidence does not justify a change.
- **Insufficient evidence:** state what observation would resolve the decision.

Use the evidence protocol when research can change the selected path.

Continue when exactly one path and its authority are clear.

## 4. Persist authorized outcomes

For an accepted automatic rule, update the bounded plan field and `Decisions`, then read both back. For a material recommendation, make no mutation until the athlete confirms it; after confirmation, hand the authorized design change to `training-design`.

Finish when the athlete receives the verified trend, the decision, its confidence, and the next observable checkpoint without overstating the data.
