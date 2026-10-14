# Local retail outbound campaign — list building, competitor scraping, and messaging with Guru

- **Date:** Aug 17, 2026 11:19 AM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/67b03684-d5ba-4ea4-aa03-99b4913c4cb2
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Campaign Overview

- Outbound campaign targeting brands not visible on AI, while competitors are
- Core message: “Your competitors are getting cited by AI, not you”
- Two brand segments:
  - Local (restaurants, bars, chai shops): competitors are city-level
  - Global/larger retailers: broader competitive set
- Initial focus: local Indian retail in Pune and Mumbai

# Target List (Subham, Next Hour)

- Pull 100-200 companies from Google Maps (Pune + Mumbai)
- Criteria: mid-to-large size, must have a domain/website
- Deliverables per company:
  - Brand name
  - Domain
  - City/location
- Scrape website for email, phone, Instagram handle using Firecrawl or Apify
- Hand list to Shans once ready for competitor agent to run locally

# Outreach Channels

- Instagram DM: preferred for local brands; owners likely active there
  - Find handles via scraper; send manually to first 50 (20-30 min)
  - Need to create an Instagram account (marketing@searchai) for outreach
- WhatsApp/SMS: possible via Brevo; same message as Instagram
- Email: via Smartlead (5-6k/month capacity, has sequencing built in)
  - SMTP server available for higher volume but needs engineering wrapper; deprioritized for now
- Brevo flagged as untested; can be explored later

# Agent Requirements

- Competitor agent needs a local flag (local vs. global) to surface city-level rivals
- Shans to build/run the agent on initial 10-20 companies
- Agent outputs: competitor list, personalized outreach message per channel (Instagram, WhatsApp, email)
- Once validated, run in batches of 100 every 2-3 hours on paid cloud

# Next Steps

- **Pull 100-200 local brand list (Pune + Mumbai) with domain and location** (Subham)

  Source from Google Maps; filter for mid-to-large brands with working domains. Deliver within one hour.
- **Scrape email, Instagram handle, and LinkedIn from brand websites** (Subham)

  Use Firecrawl or Apify; include all three channels to maximize outreach options.
- **Build competitor scraper agent for local brands** (Shans)

  Run on first 10-20 companies; output competitor names and personalized messages per channel.
- **Send first 50 Instagram DMs manually** (Subham)

  Create marketing@searchai Instagram account first; use personalized messages from the agent.
- **Reconnect at 4-5 PM today (17th August)**

  Review baseline list and agent output; scale batch runs if ready.
