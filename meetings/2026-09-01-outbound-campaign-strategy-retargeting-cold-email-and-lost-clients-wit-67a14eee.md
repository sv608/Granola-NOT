# Outbound campaign strategy — retargeting, cold email, and lost clients with Rukria

- **Date:** Sep 1, 2026 9:32 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/67a14eee-2188-4408-ab5c-907526c8ea41
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Current Outbound Setup (Lemlist)

- Using Lemlist for outbound, with 5 lists of 5,000–10,000 contacts each
- Messaging tailored per ICP (business analysts, QA, etc.)
- No dedicated landing pages: all CTAs directed to booking a call
- Not using the model requirements domain; using other purchased domains
- Apollo sequences currently handling post-form/booking follow-ups, but very generic (“hey, thanks for booking, text me tomorrow”)
  - Nikhil flagged this as a likely reason for declining demo bookings

# Lead Performance and Pipeline Concerns

- Last week: 4 leads total (CP + MR combined, per sheet); team reported higher
- This week (Mon–Tue): only 1 calendar booking across both business units
- Direct calendar link added to reduce friction, but bookings still not improving
- Pure cold outreach not working for MR per Nikhil; consensus to shift focus to retargeting

# Retargeting Campaign Plan (Two Parallel Campaigns)

- Two campaigns running in parallel: one for MR, one for CP
- Each campaign targets:
  - Existing opportunities (came to demo but didn’t convert)
  - Leads who filled the form but never showed up
- Same strategy applied to both segments: argument is that both had initial intent
- Lost clients (did not renew) added as a third campaign with the same approach
- Sequence: 5 emails over 15 business days
- Sender (same AE vs. new person) to be confirmed with Lord; skepticism about reusing same AE
- Two dedicated landing pages (one MR, one CP) with offer-based CTA
  - Offer options (e.g., 30-day free trial, Copilot for DevOps free) to be confirmed by Nikhil
  - Landing page structure: what’s changed, side-by-side comparison, testimonials, single CTA
- Target launch: Monday (after fine-tuning Friday)

# Cold Outreach: AI Personalization Agent

- Pure cold email to use a scraper-based AI agent for personalization
  - Scrapes LinkedIn profiles and websites to extract industry context, compliance needs, requirements
  - Generates 1–2 personalized paragraphs per email within a fixed 5-email sequence template
- Benefits: unique emails per contact, lower spam risk, better relevance
- Subham to write and fine-tune prompts for the agent
- Veda to research API scrapers and integration options in parallel
- Group to be created (Subham, Veda, Nikhil) with a brief; kickoff meeting tomorrow

# Tool Evaluation: Lemlist Alternatives

- Two tools recommended as cheaper alternatives to Lemlist:
  - Salesforce (comparable to SmartLead at \~50% of Lemlist cost)
  - Outplay Network (Subham has direct contact; \~50% discount available)
    - Features: AI writer, multichannel, LinkedIn outbound, positive/negative reply filtering, API access
- Both tools to be demoed before deciding; Subham to schedule both calls by tomorrow (2nd Sep)
  - Outplay contact: Subham schedules directly
  - Salesforce: US-based, likely 9 PM IST slot; confirm which tool to proceed with post-demo

# Next Steps

- **Share Lemlist credentials with Subham**

  Subham to review sequences and contact lists directly in the tool.
- **Upload lead lists to HubSpot, create segments and sequences (MR + CP)**

  Share sequences with Subham for review before launch.
- **Get offer options confirmed with Nikhil and share with Subham**

  4–5 options to be presented; agreed offer drives landing page content.
- **Build two landing pages: one for MR, one for CP (Subham)**

  First landing page by 2nd Sep, second by 4th Sep; final fine-tuning Friday 5th Sep, launch Monday 7th Sep.
- **Schedule Outplay and Salesforce demos (Subham)**

  Both calls by 2nd Sep; Salesforce likely 9 PM IST. Decide on tool post-demo.
- **Create group with Subham, Veda, and Nikhil for cold outreach agent**

  Send brief, book kickoff tomorrow; Veda to start researching API scrapers in parallel.
- **Confirm tomorrow&apos;s demo call time and update by morning (Subham)**

  Told contact the other party is available; any slot 5–12 PM IST works.
