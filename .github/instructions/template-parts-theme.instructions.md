---
applyTo: "parts/**/*.html,templates/**/*.html"
---

When reviewing pull requests, check added and modified template-part markup for a forbidden `theme` property.

Flag any `wp:template-part` usage that includes:
`"theme":"design-system-wordpress-theme"`

Expected guidance in review comments:
- Explain that template parts must not set this `theme` property.
- Ask to remove the `theme` attribute from the template-part comment.
- Point to the exact changed line in the PR diff.
