# 🕊️ Care Circle

A follow-up companion for church care teams. Built for the **AI for Church Hackathon** (Care & Community track).

A volunteer jots down notes after a visit, call or prayer request. Care Circle drafts, **for a human to review and send**:

- a warm follow-up message (9 languages, SMS/WhatsApp, email or card)
- next-touch schedule and scripture references
- a confidential pastor handoff brief
- an on-device follow-up tracker with overdue flags

## Responsible AI
- **Human in the loop:** nothing is ever sent automatically
- **Safety first:** crisis/abuse keywords trigger a "involve a pastor now" banner before any AI runs
- **Privacy:** phone numbers and emails are masked before AI sees notes; no server, no accounts; tracker stores only first name, action and due date, in the browser
- **Honest about AI:** drafts are labeled as AI-drafted; the model is told not to give medical, legal or counseling advice

## Live demo
https://claude.ai/artifact/R97XMFCesEibiY34UGbCrX

## Run it
Single file: `index.html`. The AI drafting uses Claude via the claude.ai artifact runtime, so it works in the live demo above. Hosting the file elsewhere (e.g. GitHub Pages) shows the UI but needs a small backend proxy to your own Anthropic API key to draft.

## Roadmap
Backend proxy, church-specific tone profiles, team accounts with consent, offline mode.
