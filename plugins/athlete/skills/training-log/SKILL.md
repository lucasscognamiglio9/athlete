---
name: training-log
description: Record completed training from natural-language or dictated reports, including retrospective sessions, multiple separable sessions, and corrections. Use when the athlete reports what they completed or asks to add, fix, or verify a training record.
---

# Training Log

Turn an athlete's report into a verified canonical record while preserving reported precision.

Before acting, read [`../../shared/coach-core.md`](../../shared/coach-core.md) and [`../../shared/canonical-file.md`](../../shared/canonical-file.md) completely and apply every invariant.

## 1. Ground the report

Read the canonical plan and relevant session history before assigning a date, session label, exercise identity, planned target, or duplicate status. Resolve each reliably separable session independently.

Continue when every target session and date is grounded in canonical state or explicitly provided by the athlete, and every possible duplicate is resolved.

## 2. Preserve the report

Separate explicit per-set values from values whose scope is unclear. Keep ranges, estimates, missing values, load notation, variants, and free-text observations as reported. Store a usable description such as “discos de 10 kg” verbatim rather than asking the athlete to normalize it. A planned set count does not prove that every planned set was completed with the one reported value.

Continue when every proposed field is traceable to the athlete's words or verified canonical state.

## 3. Resolve consequential ambiguity

Ask one compact clarification when an unknown can change the stored session. Group related mechanical fields in that question. Do not re-ask values already provided or ask for optional detail that cannot change the record.

Continue when every consequential ambiguity is either resolved or represented explicitly as missing or ambiguous under the storage contract.

## 4. Select the operation

- For a verification request, read and report the identified record without mutating it.
- For an explicit correction, update the identified existing record rather than appending a session.
- For completed training, append each resolved session that is not already present.

Retain the athlete's terminology when an activity cannot be matched confidently to the plan.

Continue when the requested read completes or the provider returns a mutation result for every intended field.

## 5. Verify the mutation

After a mutation, read each affected session through the same canonical interface. Compare date, session, activities, set or interval values, units, approximations, and notes with the resolved report.

Continue only when every intended field matches. If the write cannot be read back or differs, report it as unverified and do not advance dependent state.

## 6. Close the loop

Report what was verified, name any value left missing or approximate, and show the next session only when it comes from canonical state. Keep the response compact enough to scan after training.

Finish when the response separately identifies verified values, unresolved or approximate values, and any canonical next action.
