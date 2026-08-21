# Prompt: Regenerate the aem.live documentation catalog

Use this prompt to refresh `docs/aem-live-website/catalog-full.md` after changes on aem.live.

---

```
Rebuild the aem.live documentation catalog at /docs/aem-live-website/catalog-full.md from scratch.

1. Crawl: Fetch https://www.aem.live/sitemap.xml to get the current list of all
   pages. For each URL, fetch the page and extract its title and a one-sentence,
   neutral description of its content (parallelize via background agents in
   batches of ~45 pages if there are 100+ URLs, each writing its results to a
   scratch file, then merge).

2. Schema: For every documentation page, capture:
   - title (linked to its public URL)
   - audience: author | developer | business
   - level: core | advanced | reference | legacy
   - type: overview | tutorial | guide | reference | faq
   - description: one neutral sentence

3. Taxonomy: Classify each page into exactly one of these 15 categories
   (do NOT reproduce aem.live's own nav/URL structure — mix /docs/ and
   /developer/ pages freely within a category based on topic):
   1. Start Here — tutorials, onboarding, orientation, intro material
   2. Architecture — system architecture, content/code separation, delivery, availability
   3. Authoring — Document Authoring, Word/SharePoint, Google Drive, Sidekick
   4. AEM & Universal Editor — AEM authoring, UE, component models, AEM Assets, AEM-specific publishing
   5. Project Anatomy — repo structure, scripts, styles, config files, runtime conventions
   6. Blocks & Markup — blocks, sections, default content, semantic markup, Block Collection
   7. Content & Structured Data — spreadsheets, JSON, fragments, Content Fragments, placeholders
   8. Metadata, SEO & Search — metadata, bulk metadata, indexing, search, sitemap, redirects, localization
   9. Development & Performance — local dev, CLI, performance, Core Web Vitals, testing, coding practices
   10. Configuration & APIs — Configuration Service, Admin API, config tooling
   11. Git & Environments — Git, GitHub, BYO Git, staging, preview envs, deployment
   12. Integrations — Adobe/3rd-party integrations, Forms, analytics, BYOM, JSON2HTML
   13. CDN, Caching & Delivery — CDN setup (Adobe Managed, Cloudflare, Akamai, Fastly, CloudFront), invalidation, DNS
   14. Security — security architecture, authentication, authorization, access control
   15. Launch & Operations — go-live, production readiness, monitoring, troubleshooting

   Pages that aren't documentation (blog posts, business/marketing pages,
   community pages, navigation fragments like /gnav) go in a separate
   "Other content (non-documentation)" section at the end, with just
   title/type/description (no audience/level).

4. Write the result to /docs/aem-live-website/catalog-full.md, overwriting the
   existing file. Structure: intro + schema legend, table of contents linking
   to the 15 categories, one markdown table per category (Title | Audience |
   Level | Type | Description), then the "Other content" table.

5. Verify: every URL from the sitemap crawl appears exactly once across the
   categories + Other section (no drops, no duplicates) before finishing.
```

---

Notes:
- This re-derives everything from a fresh crawl rather than diffing against the old file, so it self-corrects for pages added, removed, or renamed on aem.live.
- Category assignments for borderline pages may shift slightly run-to-run since classification involves judgment — expected and fine for this use case.
- If aem.live's sitemap grows well past ~200 pages, increase the number of background crawl agents / batches proportionally so each stays in the 40–50 page range.
- If `catalog-full.md` is moved or renamed again, update the output path in step 1 and step 4 above to match.
