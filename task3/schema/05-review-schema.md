# 05 — Review Schema

## Medical Clinic — Patient Review Schema Implementation

---

## Review Schema Template

```json
{
  "@context": "https://schema.org",
  "@type": "MedicalClinic",
  "name": "[Clinic Name]",
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8",
    "reviewCount": "156",
    "bestRating": "5",
    "worstRating": "1"
  },
  "review": [
    {
      "@type": "Review",
      "author": {
        "@type": "Person",
        "name": "Patient Name"
      },
      "datePublished": "2026-01-15",
      "reviewBody": "Excellent medical care. Dr. Johnson was thorough and caring.",
      "reviewRating": {
        "@type": "Rating",
        "ratingValue": "5",
        "bestRating": "5"
      }
    }
  ]
}
```

---

## Review Collection Strategy

### Where to Collect Reviews
| Platform | Priority | Current Reviews | Target |
|----------|----------|----------------|--------|
| Google Business Profile | Critical | 23 | 50+ |
| Healthgrades | High | 12 | 30+ |
| Vitals | Medium | 8 | 20+ |
| Yelp | Medium | 5 | 15+ |
| Facebook | Low | 10 | 20+ |

### How to Collect Reviews
| Method | Timing | Script |
|--------|--------|--------|
| Post-visit email | 24 hours after visit | "Thank you for visiting! Would you share your experience?" |
| Text message | 48 hours after visit | "Hi [Name], how was your visit? Leave a review: [link]" |
| In-office signage | During checkout | "Loved your visit? Review us on Google!" |
| Follow-up call | 1 week after | "How are you feeling? We'd appreciate your feedback." |

---

## Review Response Templates

### Positive Review Response
```
Thank you for your kind words, [Name]! We're thrilled you had a positive 
experience with Dr. [Name] and our team. Your feedback means the world to us. 
We look forward to seeing you at your next visit!
```

### Negative Review Response
```
[Name], we're sorry to hear about your experience. Your feedback is important 
to us. Please contact us at [email/phone] so we can address your concerns 
directly and make things right.
```

---

## Review Display Best Practices

| Element | Recommendation |
|---------|---------------|
| Placement | Homepage, Doctor pages, dedicated Reviews page |
| Schema | Implement AggregateRating + Review schema |
| Freshness | Show most recent reviews first |
| Filtering | Show reviews from multiple platforms |
| Response | Respond to all reviews within 24 hours |

---

## Review Schema Checklist

- [ ] AggregateRating schema on homepage
- [ ] Individual Review schemas on review page
- [ ] Reviews displayed on doctor profiles
- [ ] Review response strategy in place
- [ ] Review collection emails automated
- [ ] Review monitoring dashboard set up

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 3*
