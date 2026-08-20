# Canonical File

Read this reference before connecting, creating, restructuring, or mutating athlete state.

## Capability first

Use the Google Sheets actions supplied by the separately installed and authorized official Google Drive plugin. Determine the current capability before a history-dependent claim or mutation:

- `read-write`: complete the requested operation and read it back.
- `read-only`: use verified state and provide a compact manual-entry summary.
- `unavailable`: keep guidance provisional and ask the athlete to install or connect Google Drive when durable state is required.
- `write-without-read-back`: report the attempted mutation as unverified and stop dependent state changes.

The connection belongs to the athlete. Treat installation, authentication, and permission confirmations as user-controlled actions.

## One live file

Resolve the exact spreadsheet ID and visible tab names from metadata. Reuse the designated file. Create one file only when discovery is sufficient and no canonical file exists. A structural change to an existing file requires a concise preview and authorization, then edits that same spreadsheet ID.

Keep four logical blocks in the file:

- `Profile`: current athlete fields that affect coaching, with value quality and update time.
- `Plan`: the active version, prescribed work, visible targets, and accepted progression rules.
- `Sessions`: completed work and the metrics needed to interpret it.
- `Decisions`: applied changes, reasons, status, and relevant provenance.

Use four tabs by those names for a new file. Reuse equivalent existing tabs when their meaning is unambiguous.

Keep the file easy to scan: one clear title, one short instruction line, one header row, frozen headers, readable widths, and restrained status colors. Formatting serves live use; it never justifies another tab, file, or field.

## Adaptive shape

Choose fields from the athlete's actual plan and decisions after discovery. Start with the smallest usable shape and add a field in place only when a real operation or decision needs it.

`Discipline` is optional descriptive context. Include it only when it disambiguates activities, rules, or metrics. A single-practice athlete normally has no discipline field or column.

For session rows, select only applicable primitives: task or activity, dose, intensity or effort, observed result, quality, and notes. Duration, distance, load, repetitions, intervals, variants, and effort scales are independent optional fields; the practice label never selects a schema family.

Preserve `confirmed`, `approximate`, `ambiguous`, and `missing` values. Keep the athlete's units and reported ranges.

## Read, write, read back

Before writing, read metadata and the smallest ranges that ground the operation, including validation or formulas that can affect it. Mutate a coherent bounded range. Then read every affected field through the same Google Sheets interface and compare it with the intended state.

Success requires the same spreadsheet ID, matching returned values, and no auxiliary file. Report mismatches or unreadable writes as unverified.
