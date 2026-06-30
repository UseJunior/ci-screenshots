# ci-screenshots

Public-by-design host for **CI / PR-review / issue screenshots** that need to
embed inline in GitHub markdown.

`raw.githubusercontent.com/UseJunior/ci-screenshots/<branch>/<path>` URLs render
natively in issue bodies, PR bodies, and comments.

## What goes here

- Post-merge smoke screenshots (`pr-<n>/postmerge-*.png`)
- Pre-merge PR-review screenshots (`pr-<n>/premerge-*.png`)
- Repro screenshots for issues we open (`issue-<slug>/*.png`)

Pairing `premerge-*` and `postmerge-*` under the same `pr-<n>/` folder lets a
reviewer eyeball pre- vs post-merge consistency.

## What does NOT go here

Ephemeral artifacts only. **Never** canonical data, customer data, secrets, or
anything you wouldn't post publicly. This repo exists specifically so that the
org's private GCS buckets and data projects never have to be made public to host
a screenshot.

Published via `~/.claude/skills/screenshot-evidence/screenshot-evidence.sh`.
