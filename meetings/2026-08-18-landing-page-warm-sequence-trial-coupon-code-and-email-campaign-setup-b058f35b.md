# Landing page warm sequence — trial, coupon code, and email campaign setup

- **Date:** Aug 18, 2026 9:34 AM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/b058f35b-049e-4cd4-9c28-a7cd77156120
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Landing Page and Trial Flow

- Warm landing page built in React, partially ported to WordPress
  - Some animations lost in migration; header still needs removal
  - Footer CTA suppressed to avoid clash with page CTA
- Trial flow change agreed: require credit card at signup, before setup
  - Current flow lets users complete full setup without a card, leading to drop-off risk
  - New flow: credit card + promo code entry immediately after email activation
  - Promo code: $0 for first month (not $1), trial begins on card entry
- Trial duration reduced from 30 to 15 days
  - Competitors mostly run 14-30 days; ShipStation likely 14 days
  - 15 days creates urgency without being too short
  - Website copy needs updating to reflect new duration

# Comparison Table and Messaging

- “Typical shipping app” label flagged as weak; should name actual competitors
  - Suggested targets: ShipStation, Shippo, and 2-3 core rivals
  - Research approach: use AI research agents to scrape competitor sites, then cross-verify manually
  - Guru has an existing analysis table as a starting point
- Key differentiators to call out above the fold:
  - Cheaper carrier rates, multi-channel sync, lower subscription fees
  - Add explicit “less expensive than competitors with same or more features” messaging
- Timeline: launch campaign Friday with current table; update with named competitors by Monday/Tuesday

# UTM Tracking and Email Sequence

- UTM source table to be created covering all traffic sources:
  - Four app stores: Shopify, Amazon, BigCommerce, and one smaller platform
  - Email campaigns (via Instantly)
  - Paid ads deprioritized for now (ads paused)
- Alok to send URLs for all marketplaces and app stores so UTM codes can be assigned
- Email sequence (warm leads): 5-6 emails drafted in Google Doc, reviewed by Thursday, live by Friday
  - Two CTAs per email: direct signup with promo code, or visit landing page

# Next Steps

- **Send warm landing page HTML to the team** (Subham)

  Needed to build the email sequence today.
- **Review landing page and fix remaining issues** (Subham)

  Quick sync after the 9:30 call to finalize the page before launch.
- **Add credit card requirement and promo code to signup flow**

  Card entry before setup screen; $0 first-month coupon applied at that step.
- **Create UTM source table and add Alok&apos;s task to the Excel tracker** (Subham)

  Alok to supply URLs for all app stores and marketplaces so UTM codes can be assigned.
- **Draft 5-6 email warm sequence in Google Doc**

  Ready for Guru review by Thursday; go live Friday.
- **Research competitor feature tables using AI scraping agents**

  Cross-verify output manually; update comparison table with named competitors by Monday/Tuesday.
