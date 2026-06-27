# 04 — Local Business Schema

## Medical Clinic — LocalBusiness + MedicalClinic Schema

---

## LocalBusiness Schema Template

```json
{
  "@context": "https://schema.org",
  "@type": "MedicalClinic",
  "name": "[Clinic Name]",
  "image": "https://www.example.com/images/clinic-main.jpg",
  "url": "https://www.example.com/",
  "telephone": "+1-[phone]",
  "email": "info@[clinic].com",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "[Street Address]",
    "addressLocality": "[City]",
    "addressRegion": "[State]",
    "postalCode": "[ZIP]",
    "addressCountry": "US"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": "[latitude]",
    "longitude": "[longitude]"
  },
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
      "opens": "08:00",
      "closes": "18:00"
    },
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": "Saturday",
      "opens": "09:00",
      "closes": "14:00"
    }
  ],
  "priceRange": "$$",
  "medicalSpecialty": ["Primary Care", "Internal Medicine", "Pediatrics"],
  "availableService": [
    {
      "@type": "MedicalProcedure",
      "name": "Primary Care Consultation"
    },
    {
      "@type": "MedicalProcedure",
      "name": "Health Screening"
    }
  ],
  "isAcceptingNewPatients": true,
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8",
    "reviewCount": "156",
    "bestRating": "5"
  },
  "sameAs": [
    "https://www.facebook.com/[clinic]",
    "https://www.instagram.com/[clinic]",
    "https://www.linkedin.com/company/[clinic]"
  ]
}
```

---

## Local SEO Checklist

| Element | Status | Action |
|---------|--------|--------|
| Google Business Profile | ✅ Claimed | Optimize with photos, services |
| NAP Consistency | ⚠️ Check | Ensure same Name, Address, Phone everywhere |
| Local Keywords | ❌ Missing | Add "[city]" to all pages |
| Location Pages | ❌ Missing | Create neighborhood pages |
| Local Backlinks | ⚠️ Low | Build local citations |
| Reviews | ⚠️ 23 reviews | Increase to 50+ |

---

## Google Business Profile Optimization

| Element | Recommendation |
|---------|---------------|
| Business Name | Exact match: "[Clinic Name]" |
| Category | Primary: "Medical Clinic" |
| Description | 750 chars with keywords |
| Services | List all services offered |
| Hours | Keep updated, especially holidays |
| Photos | 20+ high-quality photos |
| Posts | Weekly updates with offers/info |
| Q&A | Answer all questions promptly |

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 3*
