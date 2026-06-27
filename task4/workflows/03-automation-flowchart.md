# 03 — Automation Flowchart

## Startup Investment Firm — Email Funnel Visual Flowchart

---

## Complete Flowchart

```
┌─────────────────────────────────────────────────────────────────┐
│                         START                                    │
│                    User clicks ad/post                           │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    LANDING PAGE                                  │
│  "2026 Investment Strategy Quiz"                                │
│  Form: Name, Email, Experience                                  │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    INTERACTIVE QUIZ                              │
│  10 Questions: Risk, Goals, Experience, Preferences             │
│  Platform: Typeform                                             │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    DATA CAPTURE                                  │
│  Typeform → Mailchimp/HubSpot                                  │
│  Create contact + custom properties                             │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    SEGMENTATION                                 │
│                                                                │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐                     │
│  │Conservative│  │ Moderate │  │Aggressive│                     │
│  └─────┬────┘  └─────┬────┘  └─────┬────┘                     │
└────────┼──────────────┼──────────────┼─────────────────────────┘
         │              │              │
         └──────────────┼──────────────┘
                        │
                        ▼
┌─────────────────────────────────────────────────────────────────┐
│                    WELCOME EMAIL (Immediate)                     │
│  Subject: "Your 2026 Investment Strategy is Ready"              │
│  Content: Quiz results + personalized recommendations           │
│  CTA: Download Playbook                                         │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    WAIT 3 DAYS                                   │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    FOLLOW-UP 1 (Day 3)                           │
│  Subject: "3 investment mistakes to avoid"                      │
│  Content: Educational value                                     │
│  CTA: Book Consultation                                         │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    WAIT 2 DAYS                                   │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    FOLLOW-UP 2 (Day 5)                           │
│  Subject: "How [Name] grew portfolio by 34%"                    │
│  Content: Social proof / testimonial                            │
│  CTA: Start Investment Journey                                  │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    WAIT 2 DAYS                                   │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    FOLLOW-UP 3 (Day 7)                           │
│  Subject: "Last chance: Your plan expires"                      │
│  Content: Urgency + scarcity                                    │
│  CTA: Claim Personalized Plan                                   │
└─────────────────────────┬───────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────────┐
│                    SEGMENT CHECK                                 │
│                                                                │
│  ┌─────────────────┐  ┌─────────────────┐                      │
│  │ Clicked Consult │  │ No Click        │                      │
│  │ → HOT LEAD      │  │ → NEWSLETTER    │                      │
│  └────────┬────────┘  └────────┬────────┘                      │
└───────────┼────────────────────┼───────────────────────────────┘
            │                    │
            ▼                    ▼
┌───────────────────┐  ┌───────────────────┐
│  SALES FOLLOW-UP  │  │  NEWSLETTER       │
│  Personal call    │  │  Weekly updates   │
│  Consultation     │  │  Market insights  │
└───────────────────┘  └───────────────────┘
```

---

## Key Decision Points

| Point | Condition | Action |
|-------|-----------|--------|
| After Welcome | Opened? | If no, resend subject |
| After Follow-up 1 | Clicked? | Score +10 points |
| After Follow-up 2 | Consultation click? | Hot lead + sales task |
| After Follow-up 3 | Any engagement? | Move to newsletter |

---

## Automation Rules

| Rule | Trigger | Action |
|------|---------|--------|
| Hot Lead | Clicked consultation CTA | Add tag, notify sales |
| Re-engagement | No opens in 7 days | Send re-engagement email |
| Unsubscribe | Clicked unsubscribe | Remove from all workflows |
| Preference Update | Updated quiz | Refresh segmentation |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 4*
