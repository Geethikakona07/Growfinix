# 02 — Medical FAQ Schema

## Medical Clinic — FAQ Schema Implementation

---

## FAQ Schema Template

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What services does [Clinic Name] offer?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Clinic Name] offers comprehensive medical services including primary care, preventive health screenings, chronic disease management, women's health, pediatric care, and specialist consultations."
      }
    },
    {
      "@type": "Question",
      "name": "Do I need an appointment to visit [Clinic Name]?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "While walk-ins are welcome for urgent care, we recommend scheduling an appointment for routine check-ups and consultations. You can book online or call our office."
      }
    },
    {
      "@type": "Question",
      "name": "What insurance does [Clinic Name] accept?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "We accept most major insurance plans including Medicare, Medicaid, Blue Cross Blue Shield, Aetna, Cigna, and UnitedHealthcare. Please contact us to verify your specific plan."
      }
    },
    {
      "@type": "Question",
      "name": "What are the clinic hours?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "We are open Monday-Friday 8:00 AM - 6:00 PM, Saturday 9:00 AM - 2:00 PM, and closed on Sundays. Urgent care hours may vary."
      }
    },
    {
      "@type": "Question",
      "name": "How do I prepare for my first visit?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Please bring your insurance card, photo ID, list of current medications, and any relevant medical records. Arrive 15 minutes early to complete paperwork."
      }
    }
  ]
}
```

---

## FAQ Content by Page

### Homepage FAQs
1. What makes [Clinic Name] different from other clinics?
2. Do you accept new patients?
3. What are your office hours?
4. How do I schedule an appointment?
5. Do you offer telemedicine appointments?

### Services Page FAQs
1. What medical services do you provide?
2. Do you offer preventive health screenings?
3. Can you manage chronic conditions like diabetes?
4. Do you provide specialist referrals?
5. What diagnostic tests are available?

### Doctor Page FAQs
1. What are the doctor's qualifications?
2. How many years of experience does the doctor have?
3. What conditions does the doctor treat?
4. Is the doctor accepting new patients?
5. How can I book an appointment with the doctor?

---

## FAQ Best Practices

| Rule | Detail |
|------|--------|
| Questions | Use real patient questions |
| Answers | Provide complete, helpful answers |
| Length | 50-150 words per answer |
| Keywords | Include relevant keywords naturally |
| Schema | Validate with Google Rich Results Test |
| Placement | Above the fold or in dedicated section |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 3*
