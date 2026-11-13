# Third-Party Reuse Policy (rev 3, effective 2026-09-01)

## 1. Evidence standard

Every register entry must name the direct source that actually hosts the artifact
bytes. Attribution prose on an artifact card is a lead, not evidence. A candidate
source is confirmed only when it contains a file with the same name and identical
contents as one of the artifact's files; record that file name as the fingerprint.

## 2. License classes and required actions

| License declared by the confirmed source | status | action |
| --- | --- | --- |
| MIT, BSD-2-Clause, BSD-3-Clause, Apache-2.0, ISC | approved | attribute_in_notice |
| GPL-2.0, GPL-3.0, LGPL-2.1, LGPL-3.0, AGPL-3.0, MPL-2.0, CC-BY-SA-3.0, CC-BY-SA-4.0 | review_required | open_legal_review |
| no declaration, unknown, unspecified | blocked | remove_or_replace |
| any other identifier | review_required | open_legal_review |

## 3. Recording rules

- Read the license from the confirmed source's own README (YAML front matter or a
  dedicated license section). Never inherit a license from the mirror that copied it.
- Use the SPDX-style identifier exactly as the source writes it, lower-cased.
- `fingerprint_file` is the exact file name used for the match, including extension.
- `reviewed_on` is the date the entry was decided (YYYY-MM-DD).
