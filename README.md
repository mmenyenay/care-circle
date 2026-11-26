# 🕊️ Care Circle

A follow-up companion for church care teams. Built for the **AI for Church Hackathon** (Care & Community track).

A volunteer jots down notes after a visit, call or prayer request. Care Circle drafts, **for a human to review and send**: a follow-up message (9 languages; SMS/WhatsApp, email or card), next touches, scripture references, a confidential pastor handoff brief, plus an on-device follow-up tracker.

## Responsible AI
- **Human in the loop:** nothing is ever sent automatically
- **Safety first:** crisis/abuse keywords trigger an "involve a pastor now" banner before any AI runs
- **Privacy:** phone numbers and emails are masked in the browser before notes leave the device; no accounts, no database; the tracker stores only a first name, action and date in the browser
- **Honest about AI:** drafts are labeled AI-drafted; the model is told not to give medical, legal or counseling advice

## Stack
Static `index.html` + one Vercel serverless function (`api/draft.js`) that calls Gemini or Groq. API keys stay in Vercel environment variables.

## Deploy
1. Import this repo in Vercel (framework preset: Other)
2. Add env var `GEMINI_API_KEY` (or `GROQ_API_KEY`); optional `GEMINI_MODEL` / `GROQ_MODEL`
3. Deploy

## Roadmap
Church tone profiles, team accounts with consent, offline mode, native-speaker review of local-language drafts.
