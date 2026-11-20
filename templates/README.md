# Free n8n Workflow Templates (Official EU & French Open Data)

Ready-to-import n8n JSON blueprints powered by deterministic, zero-proxy Apify Actors.

| Workflow Template | What It Automates | Powered By |
|---|---|---|
| [`n8n_eu_public_tenders_slack_sheets.json`](./n8n_eu_public_tenders_slack_sheets.json) | Daily 08:00 watch on EU TED v3 (27 EU countries) + French BOAMP tenders with buyer email/phone -> upserts Google Sheets + posts Slack alerts | [`yannabadie/eu-public-tenders-ted-boamp`](https://apify.com/yannabadie/eu-public-tenders-ted-boamp) |
| [`n8n_french_company_kyc_enrichment.json`](./n8n_french_company_kyc_enrichment.json) | Webhook taking a SIREN list -> enriches SIRENE/RNE + VAT + BODACC insolvency history -> routes `high_risk` / `closed` entities to Slack compliance alerts | [`yannabadie/french-company-intelligence-mcp`](https://apify.com/yannabadie/french-company-intelligence-mcp) |

## Quick Setup (2 minutes)

1. Download the `.json` file above and click **Import from File** in n8n.
2. Set `APIFY_TOKEN` (from your free Apify account — includes `$5/mo` free usage credit) and optional `SLACK_WEBHOOK_URL` in n8n environment variables.
3. Adjust CPV codes, countries, or SIREN inputs and activate the workflow.
