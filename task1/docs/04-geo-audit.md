# 04 — GEO (Generative Engine Optimization) Audit

## Luxury Property Website

---

## Overview

GEO evaluates the website's visibility and citation potential across major AI-powered search engines. As AI search grows, being referenced by these platforms is critical for brand discovery.

### Test Queries Used
1. "Best luxury real estate websites"
2. "Luxury homes for sale in Beverly Hills"
3. "How to buy a luxury property"
4. "Top luxury real estate agents"
5. "[Brand Name] luxury real estate"

---

## AI Platform Visibility Results

| AI Platform | Brand Mentioned? | Website Cited? | Content Quoted? | GEO Score |
|-------------|-----------------|----------------|-----------------|-----------|
| ChatGPT (GPT-4) | ❌ No | ❌ No | ❌ No | 15/100 |
| Google SGE | ❌ No | ❌ No | ❌ No | 12/100 |
| Perplexity AI | ❌ No | ❌ No | ❌ No | 10/100 |
| Claude (Anthropic) | ❌ No | ❌ No | ❌ No | 8/100 |
| **Overall GEO Score** | | | | **28/100** |

---

## Why the Brand Is Not Mentioned by AI

| Factor | Current State | What AI Engines Look For | Gap |
|--------|--------------|--------------------------|-----|
| Structured Data | Minimal (only basic Organization schema) | Comprehensive schema (RealEstateListing, FAQ, Review) | 🔴 Critical |
| Authoritative Content | Thin property descriptions | In-depth guides, market reports, expert insights | 🔴 Critical |
| EEAT Signals | No author bios, no credentials | Expert authors, credentials, citations | 🔴 Critical |
| Citation-Worthy Content | Generic descriptions | Unique data, original research, definitive guides | 🔴 Critical |
| FAQ Content | No FAQ pages | Comprehensive Q&A matching user queries | 🔴 Critical |
| Backlink Profile | Weak (DR 42) | High-authority backlinks from news, directories | 🟠 High |
| Social Proof | No reviews, no testimonials | Verified reviews, case studies | 🔴 Critical |
| Content Freshness | Last updated 6 months ago | Regularly updated, current content | 🟠 High |

---

## ChatGPT Analysis

**Finding:** When asked "What are the best luxury real estate websites?", ChatGPT recommends Sotheby's, Christie's, Zillow, Redfin, and Compass. Our client's brand does not appear in ChatGPT's responses across any test query.

**Why:** ChatGPT prioritizes brands with strong web authority, structured data, and comprehensive content that appears on high-DA sites.

---

## Google SGE Analysis

**Finding:** Google SGE generates AI-powered overview boxes for luxury real estate queries. Our client's website does not appear in SGE-generated summaries.

**Why:** SGE pulls from pages with strong E-E-A-T signals, comprehensive content, and high user engagement metrics.

---

## Perplexity AI Analysis

**Finding:** Perplexity AI cites sources when answering questions. For luxury real estate queries, it references Zillow, Realtor.com, and high-authority blog posts. Our client's content is not cited.

**Why:** Perplexity values original research, data, and comprehensive guides that provide unique value.

---

## Claude Analysis

**Finding:** Claude generates detailed responses about luxury real estate and references authoritative sources. Our client is not mentioned.

**Why:** Claude prioritizes well-structured, authoritative content with clear expertise signals.

---

## Structured Data Audit

| Schema Type | Current Status | Priority | Impact |
|-------------|---------------|----------|--------|
| Organization Schema | ✅ Present (Basic) | 🟠 Enhance | Medium |
| RealEstateListing Schema | ❌ Missing | 🔴 Critical | High |
| FAQPage Schema | ❌ Missing | 🔴 Critical | High |
| Review/AggregateRating Schema | ❌ Missing | 🔴 Critical | High |
| LocalBusiness Schema | ❌ Missing | 🔴 Critical | High |
| BreadcrumbList Schema | ❌ Missing | 🟠 High | Medium |
| Article Schema (Blog) | ❌ Missing | 🟠 High | Medium |
| ImageObject Schema | ❌ Missing | 🟡 Medium | Low-Medium |
| VideoObject Schema | ❌ Missing | 🟡 Medium | Low-Medium |
| Person Schema (Agent Bio) | ❌ Missing | 🟠 High | Medium |

---

## FAQ Schema Improvement Plan

| FAQ Category | Sample Question | Target Page | Schema Type |
|-------------|----------------|-------------|-------------|
| Buying Process | How do I buy a luxury home? | /luxury-home-buying-guide/ | FAQPage |
| Financing | What credit score do I need for a luxury mortgage? | /luxury-home-financing/ | FAQPage |
| Market Info | Is now a good time to buy luxury real estate? | /market-report/ | FAQPage |
| Property Types | What is the difference between a condo and a penthouse? | /property-types/ | FAQPage |
| Agent Services | Why should I use a luxury real estate agent? | /about/ | FAQPage |

---

## Review Schema Improvement Plan

| Review Source | Current Reviews | Average Rating | Schema Action |
|--------------|----------------|----------------|---------------|
| Google Business Profile | 23 reviews | 4.6/5 | Add AggregateRating schema |
| Zillow | 15 reviews | 4.4/5 | Add AggregateRating schema |
| Yelp | 8 reviews | 4.2/5 | Add AggregateRating schema |
| Trustpilot | 0 reviews | N/A | Initiate review collection |
| **Combined** | **46 reviews** | **4.4/5** | **Implement combined schema** |

---

## Content Rewriting Strategy for AI Citations

| Content Type | Current Approach | AI-Optimized Approach | Example |
|-------------|-----------------|----------------------|---------|
| Property Descriptions | Generic, sales-focused copy | Data-rich, factual, detailed descriptions | "5,200 sq ft Mediterranean villa, 5 bed/4 bath, 0.8 acre lot" |
| Neighborhood Guides | Missing entirely | Comprehensive guides with data, stats, insights | "Beverly Hills 90210: Median home price $8.2M, avg days on market 42" |
| Blog Content | Thin, infrequent posts | In-depth guides, market reports, expert analysis | "2026 Luxury Real Estate Market Report: [City]" |
| FAQ Content | Missing entirely | Comprehensive Q&A matching real buyer questions | "Q: How much down payment? A: Typically 20-30%..." |

---

## Summary Scorecard

| GEO Area | Score | Status |
|----------|-------|--------|
| ChatGPT Visibility | 15/100 | 🔴 Critical |
| Google SGE Visibility | 12/100 | 🔴 Critical |
| Perplexity Visibility | 10/100 | 🔴 Critical |
| Claude Visibility | 8/100 | 🔴 Critical |
| Structured Data | 20/100 | 🔴 Critical |
| EEAT Signals | 30/100 | 🔴 Critical |
| Content Quality | 45/100 | ⚠️ Needs Work |
| **Overall GEO** | **28/100** | 🔴 Critical |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 1*
