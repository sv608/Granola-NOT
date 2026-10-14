# Google Ads redirect and activation journey filtering with Ajinkya

- **Date:** Oct 9, 2026 2:19 PM GMT+5:30
- **Granola note:** https://notes.granola.ai/d/2b6a829a-3ea5-44f0-aa12-4c566e262d3f
- **Participants / note owner:** Subham (note creator) from Nutsovertech <sv@nutsovertech.com>

---

# Google Ads Redirect Issue

- Redirect from Google Ads campaign hits the wrong URL (cheap shipping labels page instead of “try again”)
- Root cause: double question mark in the URL breaks UTM parameter parsing
  - Entire query string passed as a key, so UTM source (Google) is not captured correctly
  - Ajinkya confirmed: removing the extra query string allows the script to pick up UTM source as Google

# Activation Journey Filtering

- Current filter dropdown shows only one journey because only one journey is configured
  - Adding more journeys will populate more options in the dropdown
- Filtering by activation step is possible: select journey, then filter by specific step (e.g., Account Created, Configure Sales Channel, Configure Carrier)
- Demonstrated filtering by UTM source, UTM medium, activation status, and current step within Account Intelligence

# Activation Journey Data Gap

- Most OrderKup accounts are missing the “Account Created” event
  - If step 1 is not completed, accounts are marked “Not Started” and excluded from activation tracking
- Workaround: set “Configure Sales Channel” as the first step in the activation journey to capture more accounts
- Needs discussion with OrderKup on how they want to configure the activation journey going forward

# Custom Segment Created

- Ajinkya created a custom segment: “Accounts Created in Last 30 Days”
  - Accessible directly through the CRM
  - Includes key columns: UTM source, UTM medium, activation status, current step, owner name
  - Subham can reorder or add columns and save changes from within the view

# Next Steps

- **Fix Google Ads redirect URL**

  Remove the duplicate question mark so UTM source passes correctly and users land on the &quot;try again&quot; page.
- **Discuss activation journey configuration with OrderKup**

  Decide whether to set &quot;Configure Sales Channel&quot; as step 1 to capture accounts missing the &quot;Account Created&quot; event.
