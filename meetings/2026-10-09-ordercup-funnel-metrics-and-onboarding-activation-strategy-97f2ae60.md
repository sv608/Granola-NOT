# OrderCup funnel metrics and onboarding activation strategy

- **Date:** Oct 9, 2026 9:16 AM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/97f2ae60-cae6-45d3-aa14-555aed79a1a3
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Meeting Cadence and Reporting Changes

- Meeting schedule change requested: shift from Tuesday/Wednesday to Tuesday/Friday (India time)
- Hard rule proposed: if the weekly report doc is not shared at least 2 hours before the call, the call should not proceed
- Weekly report format agreed:
  - Report both last-week numbers and month-to-date (MTD) for comparison
  - Breakdown by channel: cold outbound, warm outbound, ads
  - Report rows at campaign level, not aggregate totals

# Funnel Visibility and Signup Attribution

- Signup attribution now partially solved via UTM tracking in ThriveStack
  - Can identify who signed up and from which channel
  - Ajinkya set this up; needs to be consolidated into a proper dashboard
- Demo of full signup-to-conversion journey deferred to Tuesday’s call
- Current reporting pulled from Google Analytics; loses attribution after click
  - Campaign-level data (traffic, signups, conversions) needs to come from ThriveStack’s channel performance dashboard, not GA

# UTM Tagging Issues

- Cold email campaigns not consistently tagged with UTM campaign names
  - Brevo campaigns showing as “email 203” instead of a named campaign
  - Subham fixed UTM campaign name to ordercup_cold during the call
- UTM source not populating correctly in ThriveStack account-level views
  - Source shows as “Google” in account intelligence but is blank in channel performance filters
  - Attribution is broken until source/medium/campaign are consistent across all campaigns

# ThriveStack Telemetry Gaps

- Onboarding states not flowing through correctly to ThriveStack
  - account_created event not being sent; most accounts default to “not started” in CRM
  - Signup event triggers at 0 but journey milestones are not updating
- OrderCup team believes telemetry was implemented (fires at each onboarding step)
  - Disconnect is between OrderCup and ThriveStack, not within OrderCup itself
- Action: 3-way call needed between OrderCup (Nilesh), ThriveStack, and Nutsovertech to debug
- Activation step filtering in ThriveStack broken: cannot filter accounts by “configure store” step

# Onboarding Activation Problem

- Large drop-off at step 1: users create accounts but don’t connect their e-commerce channel
  - 3-step flow: connect selling channel, connect carriers, set up printers
  - Users who don’t connect a channel are likely spam or disengaged
- Root cause framed as a product activation problem, not a customer success problem
- Three questions users need answered before connecting:
  1. Why should I connect?
  2. What will I get?
  3. Is it secure?
- Recommended in-product fix: redesign the activation screen
  - Show channel options (Shopify, Amazon, etc.) and a contextual video/demo for each
  - Video or interactive click-through should open inline, not navigate away
  - Education must happen within the first 1-2 hours; anything later is too late

# Post-Signup Follow-Up Strategy

- OrderCup current process: same-day call attempt, then email with scheduling link if no answer
  - Low conversion rate; most calls go to voicemail
- Proposed enrichment-based follow-up:
  - AI enrichment (e.g., Tavily or Claude) to research user’s store type and tailor outreach
  - Personalized CTA based on what the user actually needs, not a generic newsletter
- Two parallel workstreams agreed:
  1. In-product: redesign activation screen with videos and clear value props per step
  2. Out-of-product: enriched, journey-aware email sequences based on where users dropped off

# Keyword Intent and Landing Page Gaps

- Key signup segment: users searching “USPS cheaper alternatives”
  - OrderCup rates match Shopify for USPS, so price advantage is not a differentiator
  - Landing page needs to be honest about this and redirect to actual value props
- Recommendation: intent-specific landing pages per keyword cluster
  - Example: “migrate away from Shopify shipping” as a dedicated landing page with calculators and comparisons
  - Capture user intent at signup via URL parameter, then route to a tailored activation flow
- Current product has a single standard activation flow regardless of user intent

# Next Steps

- **Update Brevo cold email campaigns with correct UTM campaign names** (Subham)

  Use consistent naming (e.g., ordercup_cold, ordercup_warm) so campaign-level attribution flows through ThriveStack.
- **Schedule 3-way telemetry debug call with Nilesh, ThriveStack, and Nutsovertech** (Subham)

  Focus on why account_created event and onboarding milestone events are not appearing in ThriveStack.
- **Share ThriveStack telemetry screenshots with Ajinkya** (Subham)

  Show where UTM source is missing in channel performance vs. visible in account intelligence, and where activation step filtering is broken.
- **Update calendar invites to move Thursday call to Friday (India time)** (Subham)

  New cadence: Tuesday and Friday. Alok confirmed Subham owns the calendar.
- **Send weekly report with cold/warm/ads breakdown before next call**

  Include both last-week and MTD numbers; rows at campaign level. Share at least 2 hours before the call.
- **Demo full signup-to-conversion journey in ThriveStack on Tuesday&apos;s call**

  Show September/October signups, their channel source, onboarding state, and paid conversion status.
- **Share OrderCup&apos;s existing ThriveStack telemetry event definitions with Nutsovertech**

  Alok to share what signals are already implemented so gaps can be identified without redundant re-implementation.
