---
name: review-performance
description: Review ad performance for a period. Use when the user asks how their ads are doing, for a weekly or monthly report, for results by campaign, or what changed compared with the previous period.
---

1. Pick the client and ad account with `list_clients` and `list_accounts` if the user has not named them.
2. Use a period of completed days, up to 31 days. Default to the last 7 days.
3. Call `get_performance` for the period and `compare_periods` against the previous period of the same length.
4. If something moved sharply, call `find_anomalies`.
5. Answer in this order: spend, results and cost per result, what changed since the previous period, the top and bottom campaigns, one next step.

Rules:
- Use only numbers from tool results. Never estimate a missing value.
- Keep it short: a small table and three to five sentences.
- Reading data changes nothing in the ad account.
- In ChatGPT the tools have other names. Use the tool list the connector shows.
