# Prescriber competencies for reviewing and prescribing SACT

This repository holds the **Prescriber competencies for reviewing and prescribing SACT** framework, published by
the UK SACT Board. A framework is one published document written as a set
of competencies. Somebody records their progress against it in their
clinician passport in Quill.

## What is here

- `frameworks/uk_sact_board_2023.yaml` is the framework itself. Its id is
  `uk_sact_board_2023`, and every competency id in it starts with `uk_sact_board_2023_`.

## How a change reaches Quill

1. Make the change on a branch named `feature/...`, and raise the
   framework's `version` by exactly one.
2. Open a pull request. The pipeline checks the file with Quill's own
   loader, and lists every competency whose wording changed.
3. Merge it. The pipeline starts Quill's framework sync, which stores the
   new version. Every earlier version stays, because a sign-off names
   the version it was made against.

A version never goes down, and a competency id is never removed.

## Licence

For now, the wording is under the same licence as Quill Medical, the GNU Affero
General Public License version 3. See `LICENSE`.
