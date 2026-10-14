# Free-to-premium conversion funnel and onboarding setup with Saurav

- **Date:** Oct 6, 2026 11:08 AM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/9deb2295-2d63-4c02-897a-f7ccd2a21226
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Funnel Visibility and Cold Outreach Gaps

- Current cold outreach is single-touch with no follow-up sequence
- Need a full funnel approach to get prospects on a call:
  - Follow up if no reply, with a cross-offer or incentive
  - Redirect founders to their ops/backend team, who are easier to influence
- Backend teams at early-stage Shopify brands are underutilized and receptive

# Google Signup Onboarding Flow

- Organic signups are coming in but almost none convert past free tier
- Free-to-premium conversion is a known hard problem across SaaS
- Need a “rockstar” 5-step email sequence triggered at signup:
  - Personalized based on the user’s Shopify store data
  - AI agents can pull store details and send hyper-personalized outreach at signup
  - Goal: surprise users with how much is already known about their store

# CRM Integration via FreshSales

- Saurav needs real-time signup data to trigger personalized outreach
- CRM confirmed as FreshSales (not ThriveStack)
- FreshSales has APIs and SDKs; Saurav can pull data directly
- Plan: use FreshSales to research each signup’s store, then reach out with tailored messaging
- Gmail/free-domain users: agreed to keep them (some are legit small Shopify sellers)

# Event Tracking Fix

- Sign-in events currently being recorded as sign-ups, which is incorrect
- Team to fix event tracking to distinguish sign-in vs. sign-up accurately
- Past users: CSV upload with date needed as a workaround

# Brevo Inbox Setup

- Brevo does not support multiple reply-to addresses
- Workaround: Aloke connects his mailbox directly to Brevo to see replies in-platform
- Bhuvana walked Aloke through the setup (Settings &gt; Inbox)

# Next Steps

- **Grant FreshSales access to Saurav** (Aloke)

  Add access@nutsovertech to FreshSales so Saurav can generate API keys and begin CRM-driven onboarding automation.
- **Fix sign-in vs. sign-up event tracking**

  Currently recording sign-ins as sign-ups; needs to be corrected for accurate funnel visibility.
- **Plan mid and bottom-of-funnel onboarding setup** (Saurav)

  Saurav to outline the onboarding sequence plan and share update with Aloke via WhatsApp the following morning.
