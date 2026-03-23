# Amazon DSP MCP Starter Kit — Manage Amazon Demand-Side Platform with AI

[![MCP Compatible](https://img.shields.io/badge/MCP-compatible-blue)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform: Amazon DSP](https://img.shields.io/badge/Platform-Amazon%20DSP-FF9900)](https://advertising.amazon.com/solutions/products/amazon-dsp)

**Programmatic advertising powered by Amazon's shopper data — managed by AI.** Open this repo in Amp, Cursor, or VS Code and manage Amazon DSP campaigns — reach shoppers across the open web, streaming TV, and audio with Amazon's unmatched purchase-intent signals.

---

## Why Amazon DSP + AI?

Amazon DSP is the only demand-side platform with direct access to Amazon's purchase data. While Google knows what people search for and Meta knows what they like, Amazon knows what they actually *buy*. This makes Amazon DSP's targeting uniquely powerful for reaching in-market shoppers.

DSP extends beyond Amazon.com — your display, video, and audio ads appear on IMDb, Twitch, Fire TV, Ring, Alexa-enabled devices, and thousands of third-party publisher sites through Amazon Publisher Services.

The complexity barrier is high. DSP has orders, line items, creatives, supply sources, audience segments, and async reporting — all with a different API pattern than Sponsored Ads. The $35,000 minimum for self-serve access means most advertisers access DSP through agencies.

An AI agent democratizes access. It navigates the DSP API, builds audience segments from Amazon's shopper data, creates campaigns, and interprets async reports — without needing a dedicated media buyer.

**Best for:** Brand awareness, reaching Amazon shoppers off-platform, streaming TV (OTT) campaigns, enterprise brands, agencies, retargeting Amazon product viewers across the web.

---

## Quick Start (30 Seconds)

### Amp / Cursor / VS Code (Copilot)

1. **Get a free API key** at [syntermedia.ai/developer](https://syntermedia.ai/developer)
2. **Set the key:**
   ```bash
   export SYNTER_API_KEY=syn_your_key_here
   ```
3. **Open this repo** in your editor
4. **Start chatting** — MCP tools are pre-configured in `.mcp.json`

### Claude Desktop

Copy `claude_desktop_config.json` to your Claude config directory and replace the API key:

- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

---

## What You Can Do

| Capability | Example |
|-----------|---------|
| **Create DSP Orders** | "Create a DSP order for brand awareness targeting in-market kitchen appliance shoppers" |
| **Line Item Management** | "Set up display line items targeting Fire TV owners" |
| **Audience Segments** | "Build an audience of people who viewed competing products but didn't purchase" |
| **Streaming TV (OTT)** | "Launch an OTT campaign on Fire TV reaching cord-cutters aged 25-44" |
| **Retargeting** | "Retarget people who viewed my product page but abandoned without purchasing" |
| **Async Reports** | "Generate a performance report for the last 30 days by audience segment" |
| **Creative Management** | "Upload banner creatives in IAB standard sizes" |
| **Supply Source Control** | "Show my ads only on premium publisher sites — exclude user-generated content" |
| **Budget Pacing** | "Is my campaign on track to spend the full monthly budget?" |
| **Frequency Capping** | "Cap impressions to 3 per user per day across all line items" |

---

## Example Conversations

### 1. Retargeting Amazon Product Viewers Across the Web

> **You:** People view my product on Amazon but don't buy. Can I follow them around the internet with ads?
>
> **Agent:** Exactly what Amazon DSP was built for. I'll create a retargeting campaign using Amazon's Advertiser Audiences.
>
> **Audience segments:**
> - Viewed your product page (last 30 days) but didn't purchase
> - Added to cart but abandoned (last 14 days)
> - Viewed your product category but bought from a competitor (last 60 days)
>
> **Where ads will appear:**
> - Amazon.com (on-platform display)
> - IMDb, Goodreads, and Amazon-owned properties
> - Third-party websites via Amazon Publisher Services
> - Fire TV screensaver and app displays
>
> **Creative strategy:**
> - Cart abandoners: "Still thinking about [Product]? It's ready for you" with product image + Add to Cart button
> - Product viewers: "Customers like you love [Product] — 4.5★ rated" with social proof
> - Competitor shoppers: "Looking for [category]? Compare [Your Product]" with competitive positioning
>
> **Budget:** $2,000/month minimum for meaningful retargeting reach
> **Expected ROAS:** 5-12x (retargeting consistently delivers the highest ROAS in DSP)

### 2. Streaming TV (OTT) Campaign on Fire TV

> **You:** I want to run TV commercials but I can't afford traditional TV. Can Amazon DSP help?
>
> **Agent:** Yes — Amazon's streaming TV ads (OTT/CTV) reach cord-cutters on Fire TV, Freevee, and Twitch at a fraction of traditional TV costs.
>
> **How it compares:**
> | Channel | Minimum Buy | CPM | Targeting | Measurable? |
> |---|---|---|---|---|
> | Traditional TV | $50,000+ | $25-35 | Age/gender only | Nielsen estimates |
> | Amazon OTT | $5,000 | $15-25 | Amazon shopper data | Exact reach + attribution |
>
> **Your campaign plan:**
> - **Format:** 15-second and 30-second video spots
> - **Placement:** Fire TV screensaver, Freevee ad breaks, Twitch pre-roll
> - **Targeting:** In-market for your product category + household income top 30%
> - **Measurement:** Amazon can track if viewers later searched for or purchased your product on Amazon
>
> This is the only TV advertising where you can attribute a TV ad view to an Amazon purchase. Traditional TV can't do that.
>
> **Budget recommendation:** Start at $5,000/month for 2 months to gather meaningful viewthrough data.

### 3. In-Market Audience Discovery

> **You:** What audiences does Amazon DSP offer that I can't get anywhere else?
>
> **Agent:** Amazon's audience taxonomy is built on actual purchase behavior — not likes, follows, or page views. Here are the categories most relevant to your product:
>
> **In-Market Audiences (actively shopping):**
> - "Premium Kitchen Appliances" — shoppers who browsed $200+ kitchen items in the last 14 days
> - "Health-Conscious Cooking" — purchased air fryers, blenders, or organic food supplements
> - "Kitchen Upgraders" — bought 3+ kitchen items in the last 90 days
>
> **Lifestyle Audiences (behavioral patterns):**
> - "Home Chef Enthusiasts" — subscribe to cooking box services + buy premium ingredients
> - "Eco-Conscious Shoppers" — consistently choose sustainable/organic products
> - "Prime Heavy Spenders" — top 10% of Prime members by annual spend
>
> **Competitor Audiences (your competitors' customers):**
> - Viewed competitor ASIN B0XXXXXXXX in the last 30 days
> - Purchased from competing brand in the last 90 days
>
> **The game-changer:** These audiences are based on what people *bought*, not what they *said* they're interested in. An "In-Market for Kitchen Appliances" audience on Amazon is 10x more qualified than the same audience on Google or Meta.

### 4. Async Reporting and Performance Analysis

> **You:** How do I get performance reports from DSP? The dashboard is confusing.
>
> **Agent:** Amazon DSP uses async reporting — you request a report, wait for it to generate, then download the results. Let me handle that for you.
>
> Requesting your last 30 days performance report by audience segment...
>
> Report ready. Here's the summary:
>
> | Audience Segment | Impressions | Clicks | Purchases | ROAS |
> |---|---|---|---|---|
> | Product Page Retargeting | 1.2M | 3,840 | 192 | 8.4x |
> | Cart Abandoners | 340K | 1,890 | 156 | 12.1x |
> | In-Market: Kitchen | 2.8M | 5,600 | 84 | 2.3x |
> | Competitor Viewers | 890K | 2,670 | 67 | 3.1x |
> | Lifestyle: Home Chef | 1.5M | 2,250 | 31 | 1.4x |
>
> **Analysis:**
> - Cart Abandoner retargeting (12.1x ROAS) is your best performer — these are hot leads
> - Product Page Retargeting (8.4x) is your volume driver — scale this
> - In-Market: Kitchen (2.3x) is mid-funnel — acceptable for awareness
> - Lifestyle: Home Chef (1.4x) is underperforming — consider pausing or testing new creative
>
> Want me to reallocate budget from Lifestyle to Cart Abandoners?

### 5. Cross-Device Frequency Management

> **You:** I feel like I'm showing the same person too many ads. How do I control that?
>
> **Agent:** Great instinct. Over-frequency is a real problem in programmatic — it annoys users and wastes budget. Let me check your current frequency data...
>
> **Current state:**
> - Average frequency: 8.2 impressions per unique user per week
> - 15% of your audience has seen 20+ impressions (diminishing returns)
> - Cross-device overlap: 34% of users see ads on both mobile and desktop
>
> **Amazon DSP's advantage:** Because Amazon DSP can identify users across devices (via Amazon login), frequency capping works cross-device — not just per cookie. This is more accurate than most DSPs.
>
> **Recommended settings:**
> - Cap at 3 impressions per user per day (across all devices)
> - Cap at 12 impressions per user per week
> - Set line-item level caps for retargeting (higher frequency OK for warm audiences)
> - Set campaign-level caps for prospecting (lower frequency to avoid annoying strangers)
>
> I'll apply these caps and monitor for 1 week. This should reduce wasted spend by ~20% while maintaining reach.

---

## Amazon DSP Tips from the Pros

1. **Start with retargeting.** Your highest-ROAS campaigns will always be retargeting Amazon product viewers and cart abandoners. Build these first, then expand to prospecting.
2. **$35K minimum for self-serve.** Amazon DSP self-serve requires a $35,000 minimum commitment. Below that, you need an agency or Amazon's managed service. The Synter MCP works with either model.
3. **In-market audiences are gold.** Amazon's in-market audiences are based on actual purchase behavior. An "in-market for laptops" audience on Amazon includes people who browsed laptops this week — not people who liked a tech page on Facebook.
4. **Streaming TV is the fastest-growing channel.** Fire TV and Freevee ad inventory is growing rapidly. Costs are 30-40% lower than traditional CTV buys (Roku, Hulu) because it's less competitive.
5. **Use async reports, not dashboards.** The DSP dashboard shows limited data. The async reporting API provides granular breakdowns by audience, creative, supply source, and device — essential for optimization.
6. **Frequency caps save budget.** Without caps, DSP will show your ad to the same person 20+ times. Set 3/day and 12/week caps to balance reach and efficiency.
7. **Amazon Attribution closes the loop.** Use Amazon Attribution to track how your DSP ads (and other channels) drive Amazon purchases. This connects upper-funnel awareness to bottom-funnel sales.

---

## FAQ

### Is there an MCP for Amazon DSP?
Yes — this repo. It pre-configures the Synter MCP server for Amazon DSP management. Works with Amp, Cursor, VS Code, and Claude Desktop.

### What's the difference between Amazon Ads and Amazon DSP?
Amazon Ads (Sponsored Products/Brands/Display) shows ads *on* Amazon.com. Amazon DSP shows ads *across the internet* — on websites, apps, Fire TV, and streaming audio — using Amazon's shopper data for targeting.

### Do I need $35,000 to start?
For self-serve DSP access, yes — Amazon requires a $35K minimum commitment. For managed service (Amazon runs it for you), the minimum is $50K. Some agencies offer pooled DSP access at lower minimums.

### Can DSP retarget Amazon shoppers on other websites?
Yes — this is DSP's core value proposition. Someone views your product on Amazon, leaves without buying, then sees your retargeting ad on CNN.com, IMDb, or a mobile app.

### Does Amazon DSP support video ads?
Yes. DSP supports display banners, video (pre-roll, mid-roll), streaming TV (OTT on Fire TV and Freevee), and audio ads (Amazon Music free tier).

---

## Related Repos

- [amazon-ads-agent](https://github.com/Synter-Media-AI/amazon-ads-agent) — Sponsored Products/Brands/Display on Amazon.com
- [trade-desk-agent](https://github.com/Synter-Media-AI/trade-desk-agent) — Alternative programmatic DSP
- [cross-platform-ads-agent](https://github.com/Synter-Media-AI/cross-platform-ads-agent) — Multi-channel management
- [audience-sync-agent](https://github.com/Synter-Media-AI/audience-sync-agent) — Sync audiences across platforms
- [ai-creative-agent](https://github.com/Synter-Media-AI/ai-creative-agent) — Generate display & video creatives
- [shopify-agent](https://github.com/Synter-Media-AI/shopify-agent) — Sync product data

---

## License

MIT — see [LICENSE](LICENSE) for details.

Built by [Synter](https://syntermedia.ai) · [Get API Key](https://syntermedia.ai/developer) · [Documentation](https://syntermedia.ai/docs)
