# SEO Skill Prompt

You are applying the SEO Skill.

Your responsibility is to audit, improve, and standardize the application's SEO implementation without changing business logic or redesigning the user interface.

---

## Objectives

Your goals are to:

- Maximize search engine discoverability.
- Prevent duplicate content.
- Ensure consistent metadata.
- Improve indexing quality.
- Follow Google's Search Essentials.
- Produce maintainable, reusable SEO implementations.

---

## Execution Rules

Always prefer reusable solutions over page-specific implementations.

Never:

- redesign the UI
- rename routes
- change business logic
- remove existing functionality
- introduce breaking changes

Only make changes related to SEO.

---

## Workflow

Follow this order.

### 1. Discover

Inspect the application.

Identify:

- routing system
- layouts
- metadata generation
- sitemap
- robots.txt
- canonical implementation
- structured data
- Open Graph
- Twitter metadata

---

### 2. Audit

Check every route.

For each page verify:

- title
- description
- canonical
- robots
- Open Graph
- Twitter Card
- structured data
- H1
- indexing status

Detect:

- duplicate titles
- duplicate descriptions
- missing metadata
- missing canonical
- incorrect robots
- duplicate URLs
- noindex mistakes

---

### 3. Classify Routes

Categorize every route.

Public

- index

Private

- noindex

Special

- search
- preview
- drafts
- experimental

---

### 4. Standardize

Create reusable implementations whenever possible.

Examples:

- shared SEO helper
- metadata utility
- reusable components
- shared configuration

Avoid duplicated metadata.

---

### 5. Validate

Verify:

- robots.txt
- sitemap.xml
- canonical URLs
- redirects
- HTTPS
- hostname consistency

---

### 6. Structured Data

Recommend appropriate schema.

Examples:

- Organization
- WebSite
- SoftwareApplication
- Product
- Article
- FAQPage
- BreadcrumbList
- TechArticle

Only apply schemas that match the content.

---

### 7. Report

Produce a concise report.

Include:

## Summary

Overall SEO health.

## Issues

List every issue found.

## Improvements

Explain each improvement.

## Files Changed

List modified files.

## Remaining Recommendations

List optional future improvements.

---

## Principles

Prefer:

- reusable code
- automation
- consistency
- maintainability
- standards compliance

Avoid:

- duplicated configuration
- hardcoded metadata
- page-specific hacks
- framework-specific assumptions

---

## Success Criteria

The task is complete when:

- Every public page has valid metadata.
- Every public page has a canonical URL.
- Private pages are not indexed.
- Sitemap is valid.
- robots.txt is valid.
- Structured data is appropriate.
- Duplicate URLs are resolved.
- The implementation is reusable.
- The final report is generated.    