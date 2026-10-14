# Connector newsletter feedback and outbound strategy refinement

- **Date:** Oct 9, 2026 10:32 AM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/765558b2-8520-4128-bb7e-a2112544bead
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

### Connector Newsletter: Engaged Users

- Positive signal: Hamza confirmed strong connection rate and relevant phone numbers on the Brevo newsletter
- Priority 1: clean up and enrich the engaged users list
  - Separate out all who have engaged so far, with company details
  - Create an enterprise installation-specific newsletter, linked back to the enterprise page
- Filter bot clicks from genuine opens/clicks
  - Add UTM IDs (Master ID approach, as done in Brevo) to track real engagement
- Engaged users who click through: send details to Graphite

### ICP Refinement and Cold Outbound

- ICP now has three major categories: enterprise, SME, retail buyers
  - Enterprise focus: 500+ employee companies in energy/oil, banking (in-house needs), sectors without reliable internet
  - Separate campaigns for: resellers, government resellers, telecom expense managers
- ICP is not yet fully clear internally; team instructed to say so rather than default to “yes”
- Action: log into HubSpot, pull leads in deal stage, run reverse enrichment
  - Deal sizes visible there ($3K, $5K, $8K, $10K range) will sharpen the real ICP
- Houston Galveston government lead spotted; pull more government-type leads from HubSpot as a template
  - Use ChatGPT to find more leads like these in the infrastructure space
- New users: add 2,000-3,000 per week max, with full enrichment and cleanup before adding to newsletter
- Cold outbound strategy: test multiple ICP + angle permutations rapidly
  - Guru’s emails flagged as missing both ICP targeting and angles
  - Subham to draft new angles and sequences to test
- ThriveStack data: Subham to revalidate the 12K dataset (low confidence in current data)
  - Alok’s data suspected to be Shopify-heavy; Shopify store owners are not the target
  - Target: Amazon/Walmart sellers and e-commerce businesses without a Shopify store
  - Scraper City suggested as a source to find non-Shopify e-commerce leads

### Team Roles and Next Steps

- Bhuvna: removed from ThriveStack involvement for now; Subham to handle directly with Ajinkya
- Bhuvna’s task today: wrap up newsletter work by 4-5 PM, then write a list of tools and tasks she understands and is confident in (pen and paper or phone notes over the weekend)
- Analytics training flagged as critical for Bhuvna: complete basic analytics training before Monday
- Data tooling and integrations ownership: fully Subham’s responsibility
- Ads priorities: Subham to follow up with Pravesh, no other action needed there

### Next Steps

- **Pull and enrich engaged users list from HubSpot deal stage** (Subham)

  Run reverse enrichment on deal-stage leads to confirm exact ICP; note deal sizes.

- **Create enterprise installation-specific newsletter segment** (Subham)

  Separate engaged users, enrich, and link back to the enterprise page.

- **Add UTM/Master IDs to newsletter links**

  Filter bot clicks from genuine opens and click-throughs, as done previously in Brevo.

- **Pull government-type leads from HubSpot and find similar via ChatGPT** (Subham)

  Use Houston Galveston lead as the template; expand cold outbound list in the infrastructure space.

- **Draft new outbound angles and sequences for ThriveStack** (Subham)

  Revalidate the 12K dataset first; target non-Shopify e-commerce sellers (Amazon, Walmart).

- **Write list of tools and tasks she is confident in** (Bhuvna)

  To be done over the weekend; basis for scoping her work going forward.
