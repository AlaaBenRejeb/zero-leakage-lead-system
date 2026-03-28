# Zero Leakage Lead System

AI-powered lead qualification system for UAE real estate agencies.

## Structure

```
zero-leakage-lead-system/
├── optin-page/          # Landing page (Vercel static)
│   ├── index.html
│   └── vercel.json
├── pdf-api/             # Serverless HTML→PDF API (Vercel function)
│   ├── api/
│   │   └── pdf.js
│   ├── package.json
│   └── vercel.json
└── .gitignore
```

## Live URLs

- Optin page: https://zero-leakage-optin-hg1fj6tr6.vercel.app
- PDF API: https://zero-leakage-pdf.vercel.app/api/pdf

## PDF API Usage

```bash
POST https://zero-leakage-pdf.vercel.app/api/pdf
Content-Type: application/json

{ "html": "<h1>Your HTML</h1>", "filename": "audit-report" }
```

Returns a binary PDF file.

## Make.com Scenario

Scenario ID: 4556393 (eu1.make.com)

### Pending setup
- Module 2 → Google Sheet ID: `1kAtmyJFXQ0TPYZosKP2SzGAoqnda9O7xfdXXSV1M2RM`
- Module 5 → PDF endpoint above
- Module 7 → WhatsApp audit template name
- Module 8 → Slack channel ID
- All `REPLACE_WITH_CALENDLY_LINK` → Calendly URL
