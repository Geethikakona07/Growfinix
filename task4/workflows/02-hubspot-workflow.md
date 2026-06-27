# 02 — HubSpot Workflow

## Startup Investment Firm — HubSpot Automation Setup

---

## Workflow Overview

| Element | Detail |
|---------|--------|
| **Name** | Investment Quiz Onboarding |
| **Trigger** | Form submission (Typeform integration) |
| **Emails** | 4 (Welcome + 3 Follow-ups) |
| **Duration** | 7 days |
| **Goal** | Convert quiz takers to clients |

---

## HubSpot Setup Steps

### Step 1: Create Contact Properties

| Property | Label | Type | Group |
|----------|-------|------|-------|
| risk_tolerance | Risk Tolerance | Dropdown | Quiz Data |
| investment_goal | Investment Goal | Dropdown | Quiz Data |
| experience_level | Experience Level | Dropdown | Quiz Data |
| investment_amount | Investment Amount | Dropdown | Quiz Data |
| preferred_sectors | Preferred Sectors | Multi-select | Quiz Data |
| learning_preference | Learning Preference | Dropdown | Quiz Data |
| communication_freq | Communication Frequency | Dropdown | Quiz Data |
| biggest_concern | Biggest Concern | Dropdown | Quiz Data |

### Step 2: Create Lists

| List Name | Type | Criteria |
|-----------|------|----------|
| Quiz Completers | Active | Has quiz data |
| Conservative Investors | Active | Risk = Conservative |
| Moderate Investors | Active | Risk = Moderate |
| Aggressive Investors | Active | Risk = Aggressive |
| Hot Leads | Active | Clicked consultation |
| Engaged | Active | Opened 2+ emails |

### Step 3: Build HubSpot Workflow

```
TRIGGER: Form submission → Typeform integration

ACTION: Set contact properties from form data
- risk_tolerance = [Q1 answer]
- investment_goal = [Q2 answer]
- experience_level = [Q3 answer]
- investment_amount = [Q5 answer]
- preferred_sectors = [Q6 answers]

ACTION: Add to list "Quiz Completers"

↓ WAIT 0 minutes

EMAIL 1: Welcome Email
- Template: Welcome template
- Personalization tokens: contact.firstname, contact.risk_tolerance

↓ WAIT 3 days

BRANCH: Opened Email 1?
├── YES → Continue
└── NO → Send reminder with new subject

EMAIL 2: Follow-up 1
- Template: Educational template
- Personalization: contact.experience_level

↓ WAIT 2 days

BRANCH: Clicked any link?
├── YES → Set lead score +10
└── NO → Continue

EMAIL 3: Follow-up 2
- Template: Social proof template
- Personalization: contact.investment_goal

↓ WAIT 2 days

BRANCH: Clicked "Book Consultation"?
├── YES → Create task for sales team
│        → Move to "Hot Leads" list
└── NO → Continue

EMAIL 4: Follow-up 3
- Template: Urgency template
- Personalization: contact.risk_tolerance

↓ WAIT 1 day

ACTION: Add to Newsletter list
ACTION: Remove from "Quiz Completers"
```

---

## HubSpot Lead Scoring

| Action | Points |
|--------|--------|
| Completed quiz | +5 |
| Opened welcome email | +5 |
| Clicked email link | +10 |
| Downloaded playbook | +15 |
| Visited pricing page | +20 |
| Booked consultation | +50 |
| **Hot Lead Threshold** | **50+** |

---

## HubSpot Reporting

| Report | Metric | Target |
|--------|--------|--------|
| Workflow Performance | Completion Rate | 90%+ |
| Email Performance | Open Rate | 40%+ |
| Email Performance | CTR | 5%+ |
| Lead Conversion | Quiz → Consultation | 5%+ |
| Revenue Attribution | Closed deals | Track |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 4*
