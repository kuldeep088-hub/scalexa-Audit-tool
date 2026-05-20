# scalexa.co Audit Tool v3.0

A free, single-file SaaS audit tool for websites and Instagram profiles. Paste any URL or Instagram handle and get a deep, actionable report in seconds — no sign-up required.

## Features

### Website Audit
- **SEO Analysis** — title, meta, headings, image alt tags, canonical, structured data
- **AEO (Answer Engine Optimization)** — FAQ schema, featured snippet readiness, question-based content
- **AI Visibility Score** — how well the site appears to AI tools like ChatGPT and Perplexity
- **GEO (Generative Engine Optimization)** — local signals, entity clarity, citation readiness
- **Page Speed** — Core Web Vitals via Google PageSpeed Insights (mobile + desktop)
- **Keyword Analysis** — top keyword extraction, density, and content gaps
- **Social Presence** — detects links to Facebook, Instagram, Twitter/X, LinkedIn, YouTube, TikTok
- **Broken Links** — scans internal links and flags dead URLs
- **Competitor Compare** — audit two sites side by side

### Instagram Audit (Paid)
- Profile health score, engagement rate, bio & link-in-bio check
- **Best Time to Post** — heatmap by day and time
- **Hashtag Strategy Report** — niche-specific hashtag tiers
- **Reel vs Carousel vs Static** — content format score for your account
- **Monetization Roadmap** — income methods ranked by readiness for your follower count
- **Growth Velocity Predictor** — 3-month follower projections by posting frequency

### General
- Freemium model — free basic audit, $1 full report
- Google Sign-In after audit completion
- Live scanning overlay with real-time findings
- PDF export via browser print
- Fully responsive, dark-themed UI
- 100% client-side — no server, no database, no backend

## Tech Stack

- Plain HTML / CSS / JavaScript (single file, no build system)
- Google PageSpeed Insights v5 API
- RapidAPI (Instagram data)
- Google Identity Services (OAuth sign-in)
- CORS proxies: `allorigins.win`, `codetabs.com`

## Getting Started

No installation needed. Just open `index.html` in a browser.

```bash
git clone https://github.com/kuldeep088-hub/nexgrow-Audit-tool.git
cd nexgrow-Audit-tool
# open index.html in your browser
```

To serve locally (required for Google Sign-In):

```bash
npx serve .
# visit http://localhost:3000
```

## Deployment

Deploy instantly on Netlify:

1. Go to [netlify.com](https://netlify.com) → Add new site → Import from Git
2. Connect GitHub and select this repo
3. Click Deploy

No build command or publish directory needed.

## Configuration

Open `index.html` and update these constants near the top of the `<script>` tag:

| Constant | Description |
|---|---|
| `PAYMENT_URL` | Your Gumroad / LemonSqueezy / Stripe payment link |
| `DEFAULT_RAPID_KEY` | Your RapidAPI key for Instagram data |
| `G_CLIENT_ID` | Your Google OAuth client ID |

## License

MIT
