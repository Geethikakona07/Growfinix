# 03 — Doctor (Physician) Schema

## Medical Clinic — Physician Schema Implementation

---

## Physician Schema Template

```json
{
  "@context": "https://schema.org",
  "@type": "Physician",
  "name": "Dr. [First Name] [Last Name]",
  "image": "https://www.example.com/images/doctors/dr-[name].jpg",
  "description": "Board-certified [specialty] with [X] years of experience at [Clinic Name].",
  "url": "https://www.example.com/doctors/dr-[name]/",
  "telephone": "+1-[phone]",
  "email": "dr-[name]@[clinic].com",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "[Street Address]",
    "addressLocality": "[City]",
    "addressRegion": "[State]",
    "postalCode": "[ZIP]",
    "addressCountry": "US"
  },
  "medicalSpecialty": "[Specialty]",
  "availableService": [
    {
      "@type": "MedicalProcedure",
      "name": "[Procedure Name]"
    }
  ],
  "alumniOf": {
    "@type": "EducationalOrganization",
    "name": "[Medical School Name]"
  },
  "award": "[Board Certification]",
  "memberOf": {
    "@type": "Organization",
    "name": "[Medical Association]"
  },
  "hasCredential": [
    {
      "@type": "EducationalOccupationalCredential",
      "credentialCategory": "Board Certification",
      "recognizedBy": {
        "@type": "Organization",
        "name": "[Board Name]"
      }
    }
  ]
}
```

---

## Doctor Profile Template

### Required Fields
| Field | Example |
|-------|---------|
| Name | Dr. Sarah Johnson |
| Specialty | Internal Medicine |
| Medical School | Harvard Medical School |
| Residency | Mass General Hospital |
| Board Certification | American Board of Internal Medicine |
| Years of Experience | 15+ years |
| Languages | English, Spanish |
| Accepting New Patients | Yes |

### Profile Content Structure

```
H1: Dr. [Name] — [Specialty] in [City]

Introduction (100 words)
- Who they are
- What they specialize in
- Why patients choose them

H2: Education & Training
- Medical School
- Residency
- Fellowship (if applicable)

H2: Specialties & Expertise
- Conditions treated
- Procedures performed
- Special interests

H2: Professional Affiliations
- Medical associations
- Hospital affiliations
- Research/publications

H2: Patient Reviews
- Average rating
- Number of reviews
- Selected testimonials

H2: Book an Appointment
- CTA with contact info
```

---

## Doctor Page Checklist

- [ ] Full name and credentials displayed
- [ ] Professional headshot with alt text
- [ ] Complete biography (800+ words)
- [ ] Education and training listed
- [ ] Board certifications shown
- [ ] Specialties clearly defined
- [ ] Patient reviews displayed
- [ ] Physician schema implemented
- [ ] Internal links to services
- [ ] CTA to book appointment

---

*Document prepared: June 2026 | Digital Marketing Internship — Task 3*
