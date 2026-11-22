# AdAce Ads for Claude

AdAce Ads connects Claude to your advertising accounts. Ask about performance, find wasted spend, check conversion tracking, and propose changes that you approve before they run.

## What is inside

- **Connector:** the hosted AdAce Ads server at `https://ads.adace.website/mcp`. You sign in with OAuth and connect your own ad accounts: Google Ads, Meta (Facebook and Instagram), Microsoft Advertising, LinkedIn Ads, TikTok Ads, Snapchat Ads, Reddit Ads and ChatGPT Ads (some platforms are in early access), plus Google Analytics 4 and Search Console.
- **Skills:**
  - `starter-requests`: eight ready-made requests (spend audit, wasted budget, what to pause, week against week, negative keywords, tracking check, plan for the week, first campaign created paused).
  - `review-performance`: a short performance review for a period, with comparison to the one before.
  - `find-wasted-spend`: find spend that brings no results and list safe fixes.
  - `change-with-approval`: propose a change, show it, and apply it only after your explicit yes.

## How changes are handled

- Reading ad data changes nothing.
- Changes that only reduce spend (pauses, budget decreases, negative keywords) are applied automatically within the limits set for the client; all other changes wait for your approval. You can choose Manual only, and then every change waits.
- Google Ads changes requested from Claude are only proposals. A person approves them in the AdAce Ads web app; they are never applied automatically and cannot be approved in a chat.
- A newly connected ad account can be view-and-advice only until its owner allows changes once.

## Plans

There is a free plan with no card needed. Plans and limits: https://ads.adace.website/en/pricing

## Data

The plugin has no code of its own and stores nothing. When you use the connector, your questions and the ad data needed to answer them go to AdAce Ads (ads.adace.website), which reads your connected ad accounts through their official APIs. Privacy policy: https://ads.adace.website/en/privacy

## Help

https://ads.adace.website/en/support
