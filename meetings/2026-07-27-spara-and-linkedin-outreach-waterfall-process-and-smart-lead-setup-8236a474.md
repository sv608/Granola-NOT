# Spara and LinkedIn outreach — waterfall process and smart lead setup

- **Date:** Jul 27, 2026 11:19 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/8236a474-9953-42c7-bc54-565e91a3fb1a
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

### Context and Goal

- Subham building a waterfall enrichment process for Nutsovertech’s outbound
- Starting with Spara, focused on LinkedIn outreach first
- Other party shared their own waterfall setup as a reference

### Waterfall Enrichment Process (Their Setup)

- Priority order to minimize cost:
  1. QuickEnrich (cheapest)
  2. Clarify
  3. Surfii
  4. Apollo (most expensive, last resort)
- Developer connected all APIs and built routing logic in their CRM (Carrot)
- Known issue: occasional “dumb data” (unrequested fields returned, e.g. CTO data when not asked)
  - Still occurring even after attempted fix

### Outbound Automation Pipeline (Their Setup for Thrive Stack)

- Full automation from Carrot to Smartlead, launched last week:
  1. Companies published in Carrot
  2. Waterfall run to get enriched leads
  3. Campaign created manually in Smartlead (one manual step)
  4. Leads pushed from Carrot into Smartlead
- On push, system scrapes website and LinkedIn profile
  - Validates current employment; updates if LinkedIn shows different company
- Cold email agent drafts 4-sequence personalized emails per lead
  - Uses website data, LinkedIn data, and 4 generic offer templates
  - Emails pushed directly into Smartlead per contact

### Nutsovertech’s Plan

- Subham will build a lighter version of the waterfall (3-4 tools max)
- Will vibe-code the API integrations; escalate to Jared and Peter if dev help needed
- Non-paid clients (e.g. N, on a barter arrangement) are the reason for building in-house
  - N provides their highest subscription tier in exchange for audience-building help
- Also needs to set up Smartlead outbound campaigns for Spara contacts

### Google Analytics and Access

- Other party requested Google Analytics access for Audience Tech on their email
  - Can integrate GA directly into Carrot for audience language insights
  - No need for a separate export tool (e.g. Z1)

### Next Steps

- **Get Spara access and share contacts for LinkedIn outreach** (Subham)

  Other party needs the contact list to plug into LinkedIn campaigns; \~100/week cadence discussed.

- **Share full Spara contact export for waterfall testing** (Subham)

  Needed to run waterfall enrichment test and set up Smartlead outbound campaigns.

- **Grant Google Analytics access for Audience Tech** (Subham)

  Share access on the email ID provided so GA can be integrated into Carrot.

- **Brief Jared and Peter on the Carrot-to-Smartlead pipeline** (Subham)

  Other party offered to demo the full outbound automation process if they&apos;re interested.
