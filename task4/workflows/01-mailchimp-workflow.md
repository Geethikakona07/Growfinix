# 01 — Mailchimp Workflow

## Startup Investment Firm — Mailchimp Automation Setup

---

## Workflow Overview

| Element | Detail |
|---------|--------|
| **Name** | Investment Quiz Onboarding |
| **Trigger** | Typeform submission |
| **Emails** | 4 (Welcome + 3 Follow-ups) |
| **Duration** | 7 days |
| **Goal** | Convert quiz takers to clients |

---

## Mailchimp Setup Steps

### Step 1: Create Audience
1. Go to Audience → Audience settings
2. Name: "Investment Quiz Leads"
3. Import Typeform data

### Step 2: Create Tags
| Tag | Purpose |
|-----|---------|
| quiz-completed | Completed investment quiz |
| risk-conservative | Conservative risk profile |
| risk-moderate | Moderate risk profile |
| risk-aggressive | Aggressive risk profile |
| goal-retirement | Retirement goal |
| goal-wealth | Wealth building goal |
| goal-passive | Passive income goal |

### Step 3: Create Custom Fields

| Field | Type | Purpose |
|-------|------|---------|
| Risk Tolerance | Text | Personalization |
| Investment Goal | Text | Personalization |
| Experience Level | Text | Segmentation |
| Investment Amount | Text | Qualification |
| Quiz Score | Text | Results tracking |

### Step 4: Build Automation Workflow

```
TRIGGER: Typeform → "quiz-completed" tag added

↓ WAIT 0 minutes

EMAIL 1: Welcome Email
- Subject: Your 2026 Investment Strategy is Ready 🎯
- Template: Welcome template
- Personalization: [First Name], [Risk Level], [Goal]

↓ WAIT 3 days

CONDITION: Opened Email 1?
├── YES → Continue
└── NO → Resend with new subject line

EMAIL 2: Follow-up 1
- Subject: 3 investment mistakes to avoid in 2026
- Template: Educational template
- Personalization: [First Name], [Experience Level]

↓ WAIT 2 days

CONDITION: Clicked any link in Email 2?
├── YES → Continue (high intent)
└── NO → Continue (standard nurture)

EMAIL 3: Follow-up 2
- Subject: How [Name] grew their portfolio by 34%
- Template: Social proof template
- Personalization: [First Name], [Goal]

↓ WAIT 2 days

CONDITION: Clicked "Book Consultation"?
├── YES → Move to "Hot Leads" segment
└── NO → Continue

EMAIL 4: Follow-up 3
- Subject: Last chance: Your personalized plan expires
- Template: Urgency template
- Personalization: [First Name], [Risk Level]

↓ END

ADD TAG: onboarding-completed
MOVE TO: Newsletter segment
```

---

## Mailchimp Segments

| Segment | Criteria |
|---------|----------|
| Hot Leads | Clicked consultation CTA |
| Engaged | Opened 2+ emails |
| At-Risk | Didn't open any emails |
| Conservative | Risk = Conservative |
| Moderate | Risk = Moderate |
| Aggressive | Risk = Aggressive |

---

## Automation Performance Tracking

| Metric | Target | Tracking |
|--------|--------|----------|
| Welcome Email Open Rate | 50%+ | Campaign report |
| Follow-up Open Rate | 35%+ | Campaign report |
| Click-Through Rate | 5%+ | Campaign report |
| Consultation Requests | 5%+ | Goal tracking |
| Unsubscribe Rate | <2% | Campaign report |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 4*
