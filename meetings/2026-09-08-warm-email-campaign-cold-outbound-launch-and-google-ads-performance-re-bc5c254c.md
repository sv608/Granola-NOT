# Warm email campaign, cold outbound launch, and Google Ads performance review

- **Date:** Sep 8, 2026 10:47 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/bc5c254c-b102-4ae9-acd4-620221920da5
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Warm Email Campaign Status

- One warm-list prospect responded, said he’s restarting his business and will sign up
  - Coupon code sent, UTM link included, but signup not yet confirmed
  - Follow-up plan: if no signup within a week, call him directly
- Edge case flagged: same user had two accounts (old email closed, new email used to re-sign up)
  - No way to detect this currently
  - Plan to make email unique (not just username) to prevent future duplicates
- 15-day trial and promo code on signup page both confirmed working

# Cold Email Campaign Launch

- 12,000 verified contacts in Google Drive (from \~42,000 Apollo contacts run through Bounceify)
  - Verification was done 6-9 months ago, must be re-verified before sending
  - Brevo will shut down the entire account (not just the campaign) if bounce or spam rate exceeds \~1%
  - Rule going forward: always verify contacts immediately before adding to Brevo
- Plan: pick 1,000 contacts, re-verify, load into Brevo with updated sequence
  - Start at 50/day, monitor bounce rate; stop and re-verify if rate spikes
  - Coupon code: “ONE MONTH FREE” (all caps, all spelled out)
  - Campaign target: live by Thursday morning (10th September), US time
  - Subham on leave Wednesday; Bhuvna to execute the Brevo setup

# Google Ads Performance Review

- Current spend: \~$357/month (August), retargeting only; search ads paused \~2 months ago
- CPC very low (21-30 cents vs. $5-12 typical for US market)
- Google reported 6 conversions; real estimate \~4 (30-40% of Google-reported conversions are spam)
  - 4 conversions at $50/month avg = \~$200 first-month revenue; 6-month LTV \~$300
  - Implied ROAS \~4x, which is strong for SaaS
- Key problem: 1,678 clicks, only 6 conversions = 0.36% conversion rate
  - Target should be 1.5-2%, which would yield \~30 signups on the same budget
  - Root cause: weak landing page, not CPC or targeting
- Only 10% of eligible retargeting inventory captured; 77% of search demand lost due to low bids; 20% lost to daily budget exhaustion
- Shopify ads effectively dead: current monthly bill \~$5, ads barely showing
  - Recommendation: reduce Shopify targeting, focus on Amazon sellers and non-Shopify merchants
  - Market context: 9M Amazon sellers vs. 2-3M Shopify sellers in the US

# Ads Improvement Plan

- Immediate priority: fix landing page, then resume retargeting ads
  - Add testimonials, video, founder/product explainer to lift conversion rate
  - Proposed budget: $400-500/month for retargeting only, 1-2 month test
  - If 2-3x ROAS confirmed, consider layering search ads back in
- Offline conversion tracking not yet implemented
  - Should upload valid signups back to Google/Meta via their conversion APIs (Google offline conversions; Meta CAPI) to improve targeting signal
- ThriveStack to be connected to Google Ads for campaign-level attribution
  - Will show which accounts converted through which campaign
  - Can export GCL IDs to build lookalike audiences in Google Ads
  - Audience segments to create: single-visit, partial signup, high time-on-site

# Homepage and Landing Page Revamp

- Cold landing page currently separate from homepage; plan to eventually replace homepage with it
- Alok reviewing competitor homepages via AI analysis; will share section-by-section recommendations
- Proposed homepage structure: split into two ICPs
  - Small/individual sellers
  - High-volume sellers
  - Possible third ICP: small 3PL providers without sophisticated software
- Guru to create mockup (similar to cold landing page process) once Alok sends the brief

# Next Steps

- **Re-verify 1,000 cold contacts and load into Brevo** (Subham, Bhuvna)

  Verification is 6-9 months old; Brevo will shut the account down above \~1% bounce rate. Launch by Thursday 10th September morning, US time.
- **Send cold email sequence to Alok for review** (Guru)

  Guru to send within \~1 hour of the call so Alok can approve before Thursday launch.
- **Review cold landing page and provide feedback** (Alok)

  Deliver feedback by end of day Tuesday 8th September.
- **Send homepage section brief and AI analysis** (Alok)

  Collate competitor analysis into recommended sections; share by end of week so Guru/Subham can build a mockup.
- **Connect Google Ads to ThriveStack**

  Needed to enable campaign-level attribution and audience segment exports for retargeting.
- **Monitor Google Analytics for cold email traffic uplift** (Subham, Bhuvna)

  Track organic, direct, and branded search traffic from Thursday 10th September onward for signs of cold campaign impact.
