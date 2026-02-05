# AI-Generated Insights & Content Automation

An end-to-end n8n automation pipeline that scrapes Walmart and Amazon product data, detects emerging trends, generates marketing insights, and automatically produces styled HTML blog + Instagram content using AI.

---

## 🚀 Overview

This workflow transforms raw e-commerce product data into actionable marketing intelligence and ready-to-publish content.

Pipeline:

Input URLs → Scrape Products → Detect Trends → Generate Signals → Create Blog + Social Content → Export HTML

It is designed for:

- Home decor brands
- E-commerce marketers
- SEO strategists
- Trend research teams
- Content automation systems

---

## 🧠 Key Features

- Walmart + Amazon scraping
- Best-seller trend extraction
- AI signal generation
- Marketing insight synthesis
- Blog outline creation
- Instagram caption generation
- Styled HTML output
- Downloadable content file
- Fully automated workflow

---

## 🏗 Architecture

### Stage 1 — URL Intake

User provides:

- Walmart product URLs
- Walmart collection URLs
- Amazon product URLs
- Amazon bestseller/search URLs

The system classifies and routes links automatically.

---

### Stage 2 — Scraping Engine

Scrapes:

- Product title
- Price
- Sizes
- Colors
- Description
- Features
- Pattern/style
- Metadata

Uses:

- HTTP requests
- Cheerio HTML parsing
- Structured extraction logic

---

### Stage 3 — Data Normalization

All scraped data is merged into a unified dataset:

```
products[]
articles[]
scrape summaries
metadata
```

Additional computed fields:

- numeric price
- product category detection
- detail counts
- timestamps

---

### Stage 4 — AI Trend Detection

AI Agent analyzes product signals and generates:

```
trend_signal
competitor_signal
style_signal
```

Signals are short, structured, and actionable.

---

### Stage 5 — Content Generation

Second AI Agent converts signals into:

- Key insights
- SEO blog strategy
- Structured outline
- Styling tips
- Engagement CTA
- Instagram caption
- Styled HTML document

---

### Stage 6 — HTML Cleanup & Export

Final steps:

- Remove markdown artifacts
- Minify HTML
- Wrap DOCTYPE
- Preview output
- Download as file.html

---

## ⚙ Requirements

- n8n installed and running
- Google Gemini API credentials
- Internet access for scraping
- Node.js environment (for cheerio parsing)

Optional:

- Supabase (if storing results)
- CDN or CMS for publishing HTML

---

## ▶ How to Use

1. Import workflow JSON into n8n
2. Add your Gemini credentials
3. Trigger workflow via chat input
4. Provide URLs:

```
Amazon product: https://...
Amazon collection: https://...
Walmart product: https://...
Walmart collection: https://...
```

5. Run workflow
6. Download generated HTML

---

## 🧾 Example Input

```
Amazon product URL: https://www.amazon.com/...
Amazon collection URL: https://www.amazon.com/s?k=Best+Sellers+in+rugs
Walmart product URL: https://www.walmart.com/ip/...
Walmart collection URL: https://www.walmart.com/search?q=Best+selling+rugs
```

---

## 📤 Output

The workflow produces:

- Key trend insights
- Blog strategy outline
- Instagram caption
- Styled HTML document
- Downloadable content file

Ready for:

- Blog publishing
- CMS upload
- Email campaigns
- Social media posts

---

## 🎯 Use Cases

- E-commerce trend analysis
- Automated content marketing
- Competitor monitoring
- SEO content pipelines
- Product launch research
- Market intelligence dashboards

---

## 🔒 Notes

- Scraping depends on retailer HTML structure
- Rate limits may apply
- CAPTCHA may block heavy scraping
- Adjust wait nodes if needed

---

## 🛠 Customization Ideas

- Add Shopify integration
- Store data in Supabase
- Add Google Trends signals
- Connect to CMS auto-publishing
- Email content drafts
- Slack alerts
- Analytics dashboard

---

## 📄 License

MIT License  
Use freely, modify responsibly.

---

## 👤 Author

AI-Generated Marketing Automation Workflow  
Built with n8n + Gemini AI

---

