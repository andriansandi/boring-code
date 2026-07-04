# SEO Troubleshooting

## Excluded by noindex

Possible causes

- Meta robots noindex
- X-Robots-Tag header
- Framework configuration

Solution

- Remove unintended noindex directives.
- Keep noindex only on private pages.

---

## Duplicate without user-selected canonical

Possible causes

- Missing canonical
- Multiple URL variants
- Query parameters
- Trailing slash differences

Solution

- Add canonical URLs.
- Normalize URLs.
- Redirect duplicates.

---

## Alternate page with proper canonical

Status

Normal.

No action required unless the canonical URL is incorrect.

---

## Crawled - Currently Not Indexed

Possible causes

- Thin content
- Duplicate content
- Low-value pages

Solution

- Improve page quality.
- Strengthen internal linking.
- Increase unique content.

---

## Soft 404

Possible causes

- Empty pages
- Placeholder pages

Solution

Return either:

- Useful content
- Proper 404 status

---

## Redirect Errors

Verify:

- No redirect loops
- No redirect chains
- HTTPS redirect
- Canonical matches destination

---

## Missing Metadata

Every page should have:

- Title
- Description
- Canonical
- Robots
- Open Graph

---

## Validation Tools

Validate using:

- Google Search Console
- Rich Results Test
- PageSpeed Insights
- Lighthouse