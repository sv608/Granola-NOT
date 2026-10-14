# Outbound campaign strategy: data extraction, enrichment, and ICP segmentation with Saurav

- **Date:** Sep 23, 2026 5:42 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/8e1abe3d-6a3b-4ebd-b29d-984fa70c8365
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Outbound Strategy: ICP and Personalization Approach

- Personalization is only in subject line and preview text: sequence body stays the same across all campaigns
  - Competitors’ names and AI queries are the two key personalization variables
  - No need for deep enrichment: 2-3 relevant fields per lead is enough
- One ICP, one campaign: each ICP type gets its own independent campaign
  - ICP types vary by industry vertical (e.g., maritime, logistics, construction, supply chain for Connecta)
  - Subject line angle changes per ICP: “Additional revenue for \[industry\] projects?”
- Email sequence shortened: replies come on email 1 or email 3, so 5-step sequence is unnecessary
  - First email: personalized hook; third: direct offer
- LinkedIn must run alongside email: better response rates confirmed by external agency (Graphit/Brit’s contact)

# Data Sourcing and Enrichment Pipeline

- Step-by-step pipeline defined:
  1. Scrape companies from relevant sources (web scrape, LinkedIn, SBIR/STTR awardees, Otterly competitor data, Thomas Net, hardware accelerators, trade shows)
  2. Find corresponding contacts via Clay (Carrot)
  3. Validate via LinkedIn profile: confirm person is still in current role/company
  4. Merge website scrape data + LinkedIn data into enriched record
  5. Store everything in Clay; push to Instantly for campaign triggering
- Enrichment cost: \~$10-12 per 1,000 contacts without LinkedIn scrape; LinkedIn scrape adds \~$5 per 1,000
  - Max \~$10 per 1,000 total if LinkedIn scraping is included
- Competitor data must come from LLM (Claude): no alternative source exists
  - Claude used once per ICP to define messaging and keywords, not on a recurring per-lead basis
- Target volume: 1,000 companies scraped, yielding 3,000-4,000 enriched contacts to outreach
- Thrive Stack: copy Otterly’s method (competitor card approach) for data sourcing
- Amejaetic ICP sources identified via ChatGPT thread: SBIR awardees, hardware accelerators, crowdfunding projects, embedded electronics trade shows

# Immediate Priorities and Client Setup

- Connecta domains: buy 2 more domains now (3 total target); 5 domains, 10 mailboxes, 300 emails/day target
  - Message Nagvi group chat to purchase; Brit needs to approve landing page before cold outbound starts
  - Brit message drafted: approve landing page to start channel partner cold outbound immediately
- Thrive Stack: start data collection now using Otterly’s method; Bhuvna to update on new search angle
  - New domains to be purchased and warmed up in Smart Leads
- Amejaetic: use Order Slice / Oshiko for data; 250-500 target companies, not a large list
- Manual data collection to start immediately (Poorna to assist) while automation is being built
  - Kritesh to manually extract data for 2,000-4,000 contacts across all clients in the interim
- Omni Kavach landing page: Sameer approved; go live, then define and build inner pages
  - Check form integration before pushing live; domain redirect via GoDaddy

# Architecture and Integration

- Kritesh’s agent to integrate with Instantly directly: all enriched data (website, LinkedIn, company info) goes into Clay automatically
  - No separate data dumps: agent pushes everything into Clay on each run
- Claude used at campaign-definition level only: define messaging, angles, keywords per ICP once
  - Low-end LLM or Instantly can handle per-lead personalization from there
- Kritesh to hand off existing agents to Vaishi for integration
- Ashwin to handle backend plumbing (30-minute call scheduled)
- Claude MCP integration with Instantly: test whether it runs correctly end-to-end

# Next Steps

- **Buy 2 more Connecta domains and set up warm-up** (Subham)

  Message Nagvi group chat; use existing card or Saurav&apos;s card. New domains go into Smart Leads with same approach as Otterly/Kenny&apos;s method.
- **Prepare Thrive Stack and Order Cup data: 1,000 companies, 3-4 contacts each** (Subham)

  Start agents today; Bhuvna to assist with manual data collection using defined sources.
- **Send Brit the landing page link for approval** (Saurav)

  Approval needed before Connecta channel partner cold outbound can start.
- **Push Omni Kavach landing page live and define inner pages** (Subham)

  Sameer approved the homepage; check form integration, then message team on which inner pages to build.
- **Test Claude MCP integration with Instantly** (Subham)

  Confirm it runs end-to-end before wiring into campaign triggers.
- **Hand off existing agents to Vaishi for integration** (Kritesh)

  Kritesh to connect with Vaishi so all enrichment flows directly into Clay automatically.
