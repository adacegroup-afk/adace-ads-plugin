---
name: find-wasted-spend
description: Find ad spend that brings no results. Use when the user asks where money is wasted, which campaigns, keywords or search terms to cut, or how to lower cost per result.
---

1. Pick the client and ad account if the user has not named them.
2. Call `find_waste` for the last 30 days (or the period the user names, up to 31 days).
3. For each item give: what it is, how much it spent, what it returned, and the safe fix (pause, lower the budget, add a negative keyword).
4. Order the list by money at stake and stop after the top five unless the user asks for more.
5. Offer to turn the fixes into change proposals. Do not create any proposal until the user says yes. Continue with the change-with-approval skill.

Rules:
- Only numbers from tool results. Explain in plain words, without ad jargon.
- Do not call a campaign wasteful on too little data. Say that the data is not enough yet.
- Negative keywords exist only for Google Ads and Microsoft Advertising (`google_ads` or `microsoft_ads` with `operation: "get_search_terms"`). Do not suggest them for other platforms.
- If the question is about tracking, use `tracking_audit`. It shows the latest saved check of the site. If it answers `NOT_AUDITED`, tell the person to open the Tracking page in AdAce Ads and run "Website tracking audit".
- In ChatGPT the tools have other names (for example `find_wasted_spend` instead of `find_waste`). Use the tool list the connector shows.
