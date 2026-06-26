# 03 — Technical SEO Audit

## Luxury Property Website

---

## Robots.txt Analysis

| Directive | Current State | Assessment |
|-----------|--------------|------------|
| User-agent | * | ✅ Correct |
| Disallow /wp-admin/ | Present | ✅ Correct |
| Disallow /search/ | Missing | ❌ Should add |
| Disallow /tag/ | Missing | ❌ Should add |
| Allow /wp-admin/admin-ajax.php | Missing | ❌ Should add |
| Sitemap directive | Missing | 🔴 Critical — Must add |

### Recommended robots.txt
```
User-agent: *
Disallow: /wp-admin/
Allow: /wp-admin/admin-ajax.php
Disallow: /search/
Disallow: /tag/

Sitemap: https://www.example.com/sitemap.xml
```

---

## XML Sitemap Audit

| Check | Status | Detail |
|-------|--------|--------|
| Sitemap exists | ✅ Yes | /sitemap.xml |
| Submitted to GSC | ❌ No | Not submitted in Search Console |
| Includes all indexable pages | ❌ No | Only 189 of 312 pages included |
| Includes lastmod dates | ⚠️ Partial | Only 40% of entries have lastmod |
| No errors in sitemap | ❌ No | 12 URLs return 404/301 |
| Image sitemap included | ❌ No | Critical for image-heavy site |
| Video sitemap included | ❌ No | Missing for virtual tours |

---

## Core Web Vitals

| Metric | Current | Target | Status | Impact |
|--------|---------|--------|--------|--------|
| Largest Contentful Paint (LCP) | 4.8s | <2.5s | 🔴 Poor | High — Direct ranking factor |
| First Input Delay (FID) | 180ms | <100ms | 🟠 Needs Work | Medium — User experience |
| Cumulative Layout Shift (CLS) | 0.32 | <0.1 | 🔴 Poor | High — Visual stability |
| First Contentful Paint (FCP) | 3.2s | <1.8s | 🔴 Poor | Medium — Perceived speed |
| Time to Interactive (TTI) | 6.1s | <3.8s | 🔴 Poor | Medium — Interactivity |
| Speed Index | 5.4s | <3.4s | 🔴 Poor | Medium — Visual load |
| Total Blocking Time (TBT) | 450ms | <200ms | 🔴 Poor | Medium — Responsiveness |

---

## Page Speed Analysis

| Page | Desktop Score | Mobile Score | Load Time | Page Size |
|------|--------------|-------------|-----------|-----------|
| Homepage | 52/100 | 28/100 | 8.2s | 4.8 MB |
| Listings | 38/100 | 18/100 | 12.4s | 8.2 MB |
| Property Detail | 35/100 | 15/100 | 14.1s | 12.6 MB |
| Blog | 61/100 | 35/100 | 5.8s | 2.1 MB |
| Contact | 72/100 | 48/100 | 3.2s | 1.4 MB |

---

## Mobile Friendliness

| Check | Status | Detail |
|-------|--------|--------|
| Mobile-responsive design | ✅ Pass | Viewport meta tag present |
| Font sizes | ⚠️ Warning | Some text requires zooming |
| Tap targets | 🔴 Fail | 47% of buttons too close together |
| Horizontal scrolling | ⚠️ Warning | Issues on property detail pages |
| Mobile page speed | 🔴 Fail | Average score: 29/100 |

---

## Broken Links Audit

| Type | Count | Top Broken URLs |
|------|-------|-----------------|
| Internal 404s | 34 | /luxury-homes/sold/old-listing-123 (12 hits) |
| External 404s | 12 | /blog/partner-link-article (8 hits) |
| Image 404s | 28 | /images/properties/old-photo.jpg (15 hits) |
| **Total** | **74** | |

---

## Duplicate Content Audit

| Issue | Pages Affected | Tool | Recommendation |
|-------|---------------|------|----------------|
| Exact duplicate content | 8 page pairs | Siteliner | Implement canonical tags |
| Near-duplicate content | 23 page groups | Copyscape | Rewrite or consolidate pages |
| HTTP/HTTPS duplicates | 33 pages | Screaming Frog | Force HTTPS redirect |
| WWW/non-WWW duplicates | All pages | Screaming Frog | Set preferred domain in GSC |
| Trailing slash duplicates | 67 pages | Screaming Frog | Implement consistent URL structure |

---

## SSL & Security

| Check | Status |
|-------|--------|
| SSL Certificate | ✅ Valid |
| HTTPS Redirect | ⚠️ Partial — Some HTTP pages accessible |
| HSTS Header | ❌ Missing |
| Content Security Policy | ❌ Missing |
| X-Frame-Options | ❌ Missing |

---

## Crawl Budget Analysis

| Metric | Value | Assessment |
|--------|-------|------------|
| Pages crawled per day | 1,200 | Acceptable |
| Average crawl time | 3.2s | Good |
| Crawl errors | 74 | Needs fixing |
| Redirect chains | 12 | Should fix |
| Redirect loops | 0 | ✅ Good |

---

## Summary Scorecard

| Audit Area | Score | Status |
|------------|-------|--------|
| Robots.txt | 50/100 | ⚠️ Needs Work |
| XML Sitemap | 40/100 | ❌ Poor |
| Core Web Vitals | 20/100 | 🔴 Critical |
| Page Speed | 35/100 | 🔴 Poor |
| Mobile Friendliness | 45/100 | ⚠️ Needs Work |
| Broken Links | 60/100 | ⚠️ Moderate |
| Duplicate Content | 55/100 | ⚠️ Needs Work |
| SSL & Security | 65/100 | ⚠️ Moderate |
| Crawl Budget | 70/100 | ⚠️ Moderate |
| **Overall Technical** | **71/100** | ⚠️ Moderate |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 1*
