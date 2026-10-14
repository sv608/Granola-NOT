# Insurance regulatory framework and knowledge base data sourcing with Mayur

- **Date:** Sep 29, 2026 3:52 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/277a515d-5dae-48a9-b3e5-e77370290c27
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Insurance Knowledge Base Project

- Building a chatbot for insurance regulatory content
- Data sources needed: IRDAI regulations, master circulars, policy wordings, first-party documents
  - Estimated volume: \~200-290 IRDAI documents across 11+ categories
- Plan: send a Google Sheet listing all sources, prioritized as P1/P2/P3
  - Team to confirm which sources are needed before ingestion
- Once sources confirmed: scrape/collect docs, build knowledge base, then chatbot on top
- Knowledge graph also under consideration
  - Needs structured format: entities + relationships defined first
  - Approach: bring sample data first, then evaluate structure

# Blog Image Review (IoT Article)

- Reviewing AI-generated images for a blog: “Why IoT Projects Stall After the Hardware Prototype is Complete”
- Reference site reviewed for image style benchmarking
  - Their images: white background with brand theme color overlaid
  - Current generated images: too dark, random colors, no brand alignment

# Image Quality Issues

- Key problems identified:
  - Images too dark across multiple blocks
  - Colors don’t match any brand theme
  - Text overlaid on images is random, not derived from section content
  - Some images convey no information at a glance
- Standard set: a reader skipping text should understand the section from the image alone
- Good example noted: “6 Layers of Enterprise IoT” image, correct structure but too dark

# Image Revision Process

- Instruction to Mayur: understand the section content manually before prompting AI
  - Don’t generate randomly; give AI a clear concept and color direction
  - Use AI to extract theme/color palette from reference images first
- Workflow going forward:
  - Complete Block 2 images first
  - Get approval before proceeding to remaining blocks
  - Avoid rework: do one block right rather than revising three times

# Social Media / Client Results Discussion

- Informal discussion about reel/content performance for a restaurant client
  - Views low; organic growth not happening despite continuous posting
  - Competitor context: another agency offering 15 reels/month package
  - Current package: 10 reels/month
- Budget and pricing friction with client mentioned
  - Client not seeing results; handover or repricing being considered
  - Organic-only strategy debated vs. paid promotion

# Next Steps

- **Send Google Sheet with prioritized source list to client** (Subham)

  List all insurance data sources (P1/P2/P3) so client can confirm what&apos;s needed for the knowledge base.
- **Redo Block 2 blog images with correct brand theme and colors** (Mayur)

  Extract color palette from reference site first; get Subham&apos;s approval before moving to other blocks.
