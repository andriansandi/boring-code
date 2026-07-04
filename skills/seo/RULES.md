# SEO Rules

These rules are mandatory.

Always follow them unless explicitly instructed otherwise.

---

# General

- Follow Google Search Essentials.
- Prefer reusable implementations over page-specific solutions.
- Keep SEO configuration centralized whenever possible.
- Generate consistent metadata across the application.
- Avoid framework-specific assumptions.
- Preserve existing application behavior.

---

# Metadata

Always:

- Generate a unique title for every public page.
- Generate a unique meta description.
- Generate absolute canonical URLs.
- Use UTF-8 encoding.
- Specify the document language.

Never:

- Duplicate titles.
- Duplicate descriptions.
- Leave metadata empty.
- Generate placeholder metadata.

---

# Canonical URLs

Always:

- Use HTTPS.
- Use absolute URLs.
- Point to the preferred URL.
- Exclude query parameters.
- Exclude tracking parameters.

Never:

- Generate relative canonical URLs.
- Generate multiple canonical tags.
- Canonicalize to redirected URLs.
- Canonicalize to non-existent pages.

---

# Indexing

Public pages must:

- Use index,follow.

Private pages must:

- Use noindex,nofollow.

Never index:

- Login pages.
- Registration pages.
- Dashboards.
- Admin pages.
- Settings.
- User profiles.
- Internal tools.
- Preview pages.
- Draft content.

---

# Sitemap

Always:

- Include only canonical public URLs.
- Keep URLs absolute.
- Keep the sitemap up to date.

Never:

- Include private pages.
- Include redirects.
- Include duplicate URLs.
- Include noindex pages.

---

# robots.txt

Always:

- Reference the sitemap.
- Allow crawling of public content.
- Block private areas.

Never:

- Block CSS or JavaScript required for rendering.
- Block public pages unintentionally.

---

# Structured Data

Always:

- Use JSON-LD.
- Match visible page content.
- Use valid Schema.org types.

Never:

- Generate misleading schema.
- Duplicate schemas unnecessarily.
- Add fake ratings or reviews.

---

# Open Graph

Every public page should include:

- og:title
- og:description
- og:url
- og:type
- og:image

Twitter Card:

- summary_large_image

---

# URLs

Prefer:

- lowercase URLs
- hyphen-separated words
- clean URLs

Avoid:

- unnecessary parameters
- uppercase paths
- duplicate URL variants

---

# Accessibility

Never sacrifice accessibility for SEO.

Always:

- Use semantic HTML.
- Provide meaningful headings.
- Include image alt text.
- Maintain logical heading order.

---

# Performance

Prefer:

- server-rendered metadata
- static generation where appropriate
- optimized images
- fast loading pages

Never introduce SEO implementations that significantly reduce performance.

---

# Security

Never expose:

- private URLs
- API keys
- internal endpoints
- admin interfaces

through metadata, sitemap, or structured data.

---

# Reporting

Always provide:

- summary
- detected issues
- applied fixes
- remaining recommendations

after completing an SEO task.