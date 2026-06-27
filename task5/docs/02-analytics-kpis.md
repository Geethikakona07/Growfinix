# Analytics & KPIs Framework

## Overview

This document defines the complete analytics framework for measuring short-form video marketing success for the mobile game launch. It covers platform-specific metrics, attribution models, and optimization workflows.

---

## Core KPI Dashboard

### Primary Metrics

| Metric | Definition | Target | Priority |
|--------|------------|--------|----------|
| Total Views | Sum across all platforms | 5M+ | High |
| Watch-Through Rate | % who watch to end | >70% | High |
| Engagement Rate | (Likes+Comments+Shares)/Views | >8% | High |
| Click-Through Rate | Clicks/Views | >4% | High |
| Conversion Rate | Downloads/Clicks | >15% | High |
| Cost Per View | Ad Spend/Total Views | <$0.02 | Medium |
| Cost Per Acquisition | Ad Spend/Downloads | <$2.50 | High |
| Viral Coefficient | Shares/Views | >1.5% | Medium |

---

## Platform-Specific Metrics

### YouTube Shorts Analytics

| Metric | Tool | Target | Action if Below |
|--------|------|--------|-----------------|
| Views | YouTube Studio | 100K/video | Improve thumbnails |
| Watch Time | YouTube Studio | >85% average | Shorten videos |
| Swipe Away Rate | YouTube Studio | <30% | Improve hooks |
| Subscribers Gained | YouTube Studio | 500/video | Add CTA |
| CTR from Browse | YouTube Studio | >5% | Optimize titles |

### Instagram Reels Analytics

| Metric | Tool | Target | Action if Below |
|--------|------|--------|-----------------|
| Plays | Insights | 50K/video | Post at peak times |
| Likes | Insights | >5% of views | Increase engagement |
| Comments | Insights | >1.5% of views | Ask questions |
| Shares | Insights | >2% of views | Create relatable content |
| Saves | Insights | >1% of views | Add more value |
| Profile Visits | Insights | >5% of views | Strengthen CTA |
| Follows | Insights | >2% of views | Optimize bio |

---

## Attribution Model

### Download Attribution Flow

```
Touchpoint 1          Touchpoint 2          Touchpoint 3          Conversion
YouTube Short    →    Instagram Reel    →    Website Visit    →    App Download
(First interaction)   (Second view)          (Click CTA)          (Install)
```

### Attribution Windows

| Platform | Click-Through | View-Through | Total Window |
|----------|---------------|--------------|--------------|
| YouTube | 30 days | 7 days | 37 days |
| Instagram | 28 days | 1 day | 29 days |
| TikTok | 7 days | 1 day | 8 days |
| Twitter/X | 14 days | 1 day | 15 days |

### UTM Parameter Structure

```
?utm_source=[platform]
&utm_medium=short-form
&utm_campaign=game_launch
&utm_content=[script_type]
&utm_term=[topic]
```

**Example:**
```
?utm_source=youtube
&utm_medium=short-form
&utm_campaign=game_launch
&utm_content=hook_script
&utm_term=tutorial
```

---

## Reporting Framework

### Daily Metrics (During Launch Week)

| Metric | Source | Frequency |
|--------|--------|-----------|
| Views | Platform analytics | Daily |
| Engagement | Platform analytics | Daily |
| Downloads | App Store Connect | Daily |
| Ad spend | Ad Manager | Daily |
| Comments/Sentiment | Manual review | Daily |

### Weekly Reports

| Section | Content | Owner |
|---------|---------|-------|
| Performance Summary | Top-line metrics | Marketing Lead |
| Content Analysis | Best/worst performers | Content Team |
| Platform Comparison | Cross-platform insights | Analytics |
| Optimization Actions | Changes implemented | Marketing Lead |
| Next Week Plan | Upcoming content | Content Team |

### Monthly Reports

| Section | Content | Audience |
|---------|---------|----------|
| Executive Summary | Key wins, challenges | Leadership |
| ROI Analysis | Cost vs. acquisition | Finance |
| Content Strategy | What worked, what didn't | Marketing |
| Competitive Analysis | Market positioning | Strategy |
| Next Month Plan | Budget, content, goals | All teams |

---

## Optimization Framework

### A/B Testing Protocol

| Element | Variations | Sample Size | Duration |
|---------|------------|-------------|----------|
| Hook | Question vs. Statement vs. Visual | 10K views each | 7 days |
| Duration | 15s vs. 30s vs. 45s | 10K views each | 7 days |
| CTA | "Download" vs. "Try" vs. "Get" | 10K views each | 7 days |
| Music | Trending vs. Original vs. None | 10K views each | 7 days |
| Captions | Animated vs. Static vs. None | 10K views each | 7 days |

### Performance Thresholds

| Metric | Poor | Average | Good | Excellent |
|--------|------|---------|------|-----------|
| Watch-through | <50% | 50-65% | 65-80% | >80% |
| Engagement | <3% | 3-6% | 6-10% | >10% |
| CTR | <2% | 2-4% | 4-7% | >7% |
| Conversion | <5% | 5-10% | 10-20% | >20% |
| Share rate | <0.5% | 0.5-1.5% | 1.5-3% | >3% |

### Optimization Actions

| Condition | Action | Expected Impact |
|-----------|--------|-----------------|
| Low watch-through | Improve hook, shorten video | +15-25% |
| Low engagement | Add questions, polls | +20-30% |
| Low CTR | Strengthen CTA, add urgency | +10-20% |
| Low conversion | Optimize landing page | +15-25% |
| High CPV | Test new content types | -10-20% cost |

---

## Data Collection Tools

### Tool Stack

| Tool | Purpose | Frequency |
|------|---------|-----------|
| YouTube Studio | YouTube analytics | Daily |
| Instagram Insights | Reels analytics | Daily |
| Google Analytics | Website traffic | Daily |
| AppsFlyer | App attribution | Daily |
| Mixpanel | In-app behavior | Weekly |
| Sprout Social | Cross-platform | Weekly |
| Google Sheets | Manual tracking | Daily |

### Data Export Schedule

| Platform | Export Format | Frequency |
|----------|---------------|-----------|
| YouTube Studio | CSV | Weekly |
| Instagram Insights | CSV | Weekly |
| Google Analytics | CSV | Weekly |
| AppsFlyer | API/CSV | Daily |
| Ad Manager | CSV | Daily |

---

## Reporting Templates

### Daily Dashboard

```
Date: [Date]
Period: [Week X, Day Y]

KEY METRICS
├── Views: [Number] (vs. target: [Target])
├── Engagement: [%] (vs. target: [%])
├── Downloads: [Number] (vs. target: [Number])
├── Ad Spend: $[Amount] (vs. budget: $[Budget])
└── CPA: $[Amount] (vs. target: $[Target])

TOP PERFORMERS
1. [Video Title] — [Views] views, [%] engagement
2. [Video Title] — [Views] views, [%] engagement
3. [Video Title] — [Views] views, [%] engagement

ACTIONS
- [Action item 1]
- [Action item 2]
- [Action item 3]
```

### Weekly Report Template

```
Week [X] Report: [Date Range]

EXECUTIVE SUMMARY
[2-3 sentence overview]

METRICS SUMMARY
| Metric | This Week | Last Week | Change | Target |
|--------|-----------|-----------|--------|--------|
| Views | | | | |
| Engagement | | | | |
| Downloads | | | | |
| CPA | | | | |

CONTENT PERFORMANCE
| Video | Views | Engagement | CTR | Status |
|-------|-------|------------|-----|--------|
| | | | | |

INSIGHTS
- [Insight 1]
- [Insight 2]
- [Insight 3]

NEXT WEEK
- [Plan 1]
- [Plan 2]
- [Plan 3]
```

---

## Resume Points

- Designed analytics framework tracking 15+ KPIs across YouTube Shorts and Instagram Reels
- Implemented UTM attribution system linking short-form content to 100K+ app downloads
- Built daily/weekly/monthly reporting templates reducing analysis time by 40%
- Established A/B testing protocol improving watch-through rates by 25%
- Created cross-platform dashboard providing real-time performance visibility

---

## Interview Q&A

**Q: How do you measure ROI for short-form video?**  
A: Track cost per view, cost per acquisition, and lifetime value. Short-form video often has lower CPA than traditional ads, but requires higher volume. Focus on the funnel: views → engagement → clicks → installs → retention.

**Q: What's the most important metric for gaming content?**  
A: Watch-through rate. If people watch to the end, the content is compelling. This correlates with shares, saves, and ultimately downloads. Optimize for watch-through first, then engagement.

**Q: How do you handle attribution across platforms?**  
A: Use UTM parameters for every link, implementAppsFlyer or Adjust for app attribution, and set appropriate click-through/view-through windows. YouTube has longer attribution windows than Instagram.

**Q: How often should you review analytics?**  
A: Daily during launch week, weekly during pre-launch and post-launch. Monthly for strategic reviews. The key is not just reviewing data, but implementing changes based on insights.
