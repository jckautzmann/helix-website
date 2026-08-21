# Prompt: Regenerate the core-only aem.live catalog

Use this prompt to refresh `docs/aem-live-website/catalog-core.md` after
`docs/aem-live-website/catalog-full.md` has been regenerated (see
`catalog-full-prompt.md`).

---

```
Based on /docs/aem-live-website/catalog-full.md: keep the same structure
(title, schema legend, taxonomy table of contents, one section per category
with a table of Title | Audience | Level | Type | Description) but only keep
rows where Level = core. Drop rows with level advanced, reference, or legacy.

- Keep every one of the 15 taxonomy categories that still has at least one
  core row; drop a category section entirely only if it has zero core rows.
- Drop the "Other content (non-documentation)" section entirely — those pages
  don't carry a Level value, so none of them qualify.
- Update the intro paragraph to say this is a level=core filtered view of
  catalog-full.md, and link back to it.
- Verify: every row kept has Level = core, and the count of core rows in the
  output matches the count of level=core rows in catalog-full.md exactly
  (e.g. via grep -c '| core |' on both files).

Save the result as /docs/aem-live-website/catalog-core.md, overwriting the
existing file.
```

---

Note: "core" here is a **level** value in the catalog schema (`core` |
`advanced` | `reference` | `legacy`), not a `type` value (`overview` |
`tutorial` | `guide` | `reference` | `faq`) — the two schema fields happen to
share the string `reference` as a possible value for both, so don't confuse
"Level: reference" rows with "Type: reference" rows when filtering.
