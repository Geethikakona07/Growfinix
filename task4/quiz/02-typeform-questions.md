# 02 — Typeform Questions

## Startup Investment Firm — Typeform Setup Guide

---

## Typeform Configuration

| Setting | Value |
|---------|-------|
| Form Name | 2026 Investment Strategy Quiz |
| Theme | Professional (Blue/Green) |
| Progress Bar | Enabled |
| Button Text | "Next" / "See My Results" |
| Thank You Screen | Custom (with results) |

---

## Typeform Setup Steps

### Step 1: Create New Typeform
1. Log in to Typeform
2. Click "Create new" → "Typeform"
3. Choose "Start from scratch"
4. Name: "2026 Investment Strategy Quiz"

### Step 2: Add Welcome Screen
```
Headline: What's Your 2026 Investment Style?
Description: Answer 10 questions to get personalized investment recommendations.
Button: Start the Quiz
```

### Step 3: Add Form Fields (Contact Info)

| Field | Type | Required |
|-------|------|----------|
| First Name | Short Text | Yes |
| Email Address | Email | Yes |
| How did you hear about us? | Dropdown | No |

### Step 4: Add Quiz Questions

| Question | Type | Options |
|----------|------|---------|
| Q1: Risk Tolerance | Multiple Choice | 5 options |
| Q2: Investment Goal | Multiple Choice | 5 options |
| Q3: Experience Level | Dropdown | 5 options |
| Q4: Investment Timeline | Multiple Choice | 5 options |
| Q5: Investment Amount | Multiple Choice | 5 options |
| Q6: Preferred Sectors | Multiple Choice (Multi) | 7 options |
| Q7: Learning Preference | Multiple Choice | 5 options |
| Q8: Communication Frequency | Multiple Choice | 4 options |
| Q9: Biggest Concern | Multiple Choice | 5 options |
| Q10: Attribution | Dropdown | 7 options |

### Step 5: Add Logic Jumps
```
If Q1 = Conservative → Show "Conservative Results"
If Q1 = Moderate → Show "Balanced Results"
If Q1 = Aggressive → Show "Aggressive Results"
```

### Step 6: Add Thank You Screen
```
Headline: Your 2026 Investment Style is Ready!
Description: We've created personalized recommendations just for you.
CTA Button: "Download Your Investment Playbook"
CTA Link: [URL to download]
```

### Step 7: Connect to Email Platform
1. Go to "Integrations"
2. Connect Mailchimp or HubSpot
3. Map fields:
   - First Name → First Name
   - Email → Email
   - Q1 Answer → Risk Tolerance (custom field)
   - Q2 Answer → Investment Goal (custom field)
   - Q3 Answer → Experience Level (custom field)
   - etc.

---

## Typeform Design Tips

| Element | Recommendation |
|---------|---------------|
| Colors | Use brand colors (Blue, Green, White) |
| Background | Clean, professional image |
| Font | Sans-serif, readable |
| Images | Add relevant images to questions |
| Progress | Show progress bar |
| Mobile | Test on mobile devices |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 4*
