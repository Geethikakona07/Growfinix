# 01 — Screaming Frog Technical Audit

## Medical Clinic — Technical SEO Crawl Report

---

## Crawl Summary

| Metric | Value |
|--------|-------|
| Total URLs Crawled | 87 |
| Internal Pages | 82 |
| External Pages | 5 |
| Response Codes (2xx) | 62 |
| Response Codes (3xx) | 7 |
| Response Codes (4xx) | 18 |
| Response Codes (5xx) | 0 |
| Page Depth | 4.2 (avg) |
| Crawl Depth | 5 levels |

---

## Response Codes

| Code | Count | URLs | Priority |
|------|-------|------|----------|
| 200 OK | 62 | All indexable pages | ✅ Good |
| 301 Redirect | 5 | /old-services → /services | ✅ Good |
| 302 Redirect | 2 | /temp-page → /new-page | ⚠️ Should be 301 |
| 404 Not Found | 18 | /blog/old-post, /images/... | 🔴 Critical |
| 500 Server Error | 0 | — | ✅ Good |

---

## Broken Links (404 Errors)

| URL | Source Page | Hits | Fix Recommendation |
|-----|-------------|------|-------------------|
| /blog/old-article-1 | Homepage | 8 | 301 redirect to /blog/ |
| /images/team-photo.jpg | About | 5 | Update image path |
| /services/removed-service | Services | 12 | 301 to /services/ |
| /old-location | Contact | 3 | 301 to /contact/ |
| /blog/broken-link | Blog | 6 | Remove or fix |

---

## Redirect Chains

| Chain | Length | Recommendation |
|-------|--------|----------------|
| /old → /temp → /current | 3 hops | Redirect /old directly to /current |
| /services/v1 → /services/v2 → /services | 3 hops | Flatten to 1 redirect |
| /blog/2023/post → /blog/post-new | 2 hops | Acceptable |

---

## Missing Page Elements

| Element | Pages Missing | Impact |
|---------|--------------|--------|
| Title Tag | 3 | High |
| Meta Description | 34 | High |
| H1 Tag | 8 | High |
| H2 Tags | 23 | Medium |
| Image Alt Text | 45 | Medium |
| Canonical Tag | 12 | High |
| Open Graph Tags | 41 | Medium |
| Twitter Card Tags | 41 | Medium |

---

## Duplicate Content

| Type | Pages Affected | Recommendation |
|------|---------------|----------------|
| Exact Duplicate | 4 page pairs | Canonical tags |
| Near-Duplicate | 8 pages | Content consolidation |
| WWW/Non-WWW | All pages | Set preferred domain |
| HTTP/HTTPS | 3 pages | Force HTTPS |

---

## Image Issues

| Issue | Count | Recommendation |
|-------|-------|----------------|
| Missing Alt Text | 45 | Add descriptive alt text |
| Over 100KB | 28 | Compress images |
| Missing Width/Height | 34 | Add dimensions |
| Wrong Format (PNG vs JPG) | 15 | Convert to WebP |

---

## Page Speed Issues

| Issue | Pages Affected | Impact |
|-------|---------------|--------|
| Large CSS Files | 23 | High |
| Render-Blocking JS | 18 | High |
| Uncompressed Images | 28 | High |
| No Browser Caching | All | Medium |
| No CDN | All | Medium |

---

## Recommendations Summary

| Priority | Issue | Fix |
|----------|-------|-----|
| 🔴 Critical | 18 broken links | Fix or redirect |
| 🔴 Critical | 34 missing meta descriptions | Add to all pages |
| 🔴 Critical | 8 missing H1 tags | Add unique H1 |
| 🟠 High | 12 duplicate content pages | Canonical tags |
| 🟠 High | 45 missing alt text | Add alt text |
| 🟠 High | 23 slow pages | Optimize speed |
| 🟡 Medium | 7 redirect chains | Flatten redirects |
| 🟡 Medium | 41 missing OG tags | Add social tags |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 3*
