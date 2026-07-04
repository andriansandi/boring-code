# Examples

## Good Title

```
Pricing · Example Product
```

---

## Good Description

```
Compare plans, features, and pricing for Example Product. Choose the plan that fits your team and start building today.
```

---

## Canonical

```html
<link rel="canonical" href="https://example.com/pricing">
```

---

## Robots

Public

```html
<meta name="robots" content="index,follow">
```

Private

```html
<meta name="robots" content="noindex,nofollow">
```

---

## Open Graph

```html
<meta property="og:title">
<meta property="og:description">
<meta property="og:url">
<meta property="og:image">
<meta property="og:type">
```

---

## Twitter

```html
<meta name="twitter:card" content="summary_large_image">
```

---

## JSON-LD

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Example",
  "url": "https://example.com"
}
```

---

## robots.txt

```
User-agent: *

Allow: /

Disallow: /admin/
Disallow: /dashboard/
Disallow: /login/
Disallow: /settings/

Sitemap: https://example.com/sitemap.xml
```

---

## URL Examples

Preferred

```
https://example.com/pricing
```

Avoid

```
https://example.com/pricing/
https://example.com/pricing?utm_source=x
https://www.example.com/pricing
http://example.com/pricing
```

All variants should redirect to the preferred canonical URL.

---

## Audit Workflow

When this skill is invoked:

1. Discover all routes.
2. Classify routes as public or private.
3. Validate metadata.
4. Validate canonical URLs.
5. Validate robots directives.
6. Validate Open Graph metadata.
7. Validate structured data.
8. Validate sitemap.
9. Validate robots.txt.
10. Generate a report summarizing findings, issues, and recommended fixes.