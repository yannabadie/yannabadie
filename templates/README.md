# Free n8n Workflow Templates (9 Deterministic, Zero-Proxy Pipelines)

Ready-to-import, n8n Creator-ready JSON blueprints (each with 2 canvas Sticky Notes, validation filters, and zero hardcoded secrets) powered by deterministic, zero-proxy Apify Actors.

| Workflow Template | What It Automates | Powered By |
|---|---|---|
| [`n8n_eu_public_tenders_slack_sheets.json`](./n8n_eu_public_tenders_slack_sheets.json) | Daily 08:00 watch on EU TED v3 (27 EU countries) + French BOAMP tenders with buyer email/phone -> Google Sheets upsert + Slack alerts | [`yannabadie/eu-public-tenders-ted-boamp`](https://apify.com/yannabadie/eu-public-tenders-ted-boamp) |
| [`n8n_french_company_kyc_enrichment.json`](./n8n_french_company_kyc_enrichment.json) | Webhook taking a SIREN list -> enriches SIRENE/RNE + VAT + BODACC insolvency history -> routes `high_risk` / `closed` entities to Slack | [`yannabadie/french-company-intelligence-mcp`](https://apify.com/yannabadie/french-company-intelligence-mcp) |
| [`n8n_clinical_trials_sponsor_watch.json`](./n8n_clinical_trials_sponsor_watch.json) | Daily 08:00 watch on ClinicalTrials.gov API v2 (`Phase 2/3`, industry sponsors, contact emails/phones) -> Google Sheets + Slack | [`yannabadie/clinical-trials-api-mcp`](https://apify.com/yannabadie/clinical-trials-api-mcp) |
| [`n8n_us_npi_healthcare_leads_sheets.json`](./n8n_us_npi_healthcare_leads_sheets.json) | Extracts U.S. clinics & doctors with direct phones, fax & Authorized Officials via CMS NPPES NPI API v2.1 -> `Filter` -> Google Sheets | [`yannabadie/npi-healthcare-providers-mcp`](https://apify.com/yannabadie/npi-healthcare-providers-mcp) |
| [`n8n_pubmed_kol_literature_watch.json`](./n8n_pubmed_kol_literature_watch.json) | Weekly Monday 08:00 watch on PubMed & Europe PMC papers with author emails, linked NCT trials & open-access PDFs -> Google Sheets + Slack | [`yannabadie/pubmed-europepmc-api-mcp`](https://apify.com/yannabadie/pubmed-europepmc-api-mcp) |
| [`n8n_multi_ats_jobs_hiring_signals.json`](./n8n_multi_ats_jobs_hiring_signals.json) | Daily 08:00 B2B hiring signal monitor across 7 public ATS JSON APIs (Greenhouse, Lever, Ashby, Workable, etc.) -> Google Sheets + Slack | [`yannabadie/multi-ats-jobs-api-mcp`](https://apify.com/yannabadie/multi-ats-jobs-api-mcp) |
| [`n8n_substack_newsletter_intelligence.json`](./n8n_substack_newsletter_intelligence.json) | Daily 08:00 Substack publication & trending post tracker with engagement scoring -> Google Sheets + Slack | [`yannabadie/substack-api-mcp`](https://apify.com/yannabadie/substack-api-mcp) |
| [`n8n_website_contact_tech_enrichment.json`](./n8n_website_contact_tech_enrichment.json) | POST Webhook accepting a domain list -> enriches emails, phones, socials & 54 tech-stack signatures -> Google Sheets upsert | [`yannabadie/website-contact-tech-enricher-mcp`](https://apify.com/yannabadie/website-contact-tech-enricher-mcp) |
| [`n8n_google_news_gdelt_brand_monitor.json`](./n8n_google_news_gdelt_brand_monitor.json) | Daily 08:00 brand & media sentiment monitor merging Google News RSS + GDELT v2 `ToneChart` -> Google Sheets + Slack | [`yannabadie/google-news-gdelt-api-mcp`](https://apify.com/yannabadie/google-news-gdelt-api-mcp) |

## Quick Setup (60 seconds)

1. Download any `.json` file above and click **Import from File** in n8n.
2. Set `APIFY_TOKEN` (from your free Apify account — includes `$5/mo` free usage credit) and optional `SLACK_WEBHOOK_URL` in n8n environment variables.
3. Replace `REPLACE_WITH_GOOGLE_SHEET_ID`, customize filters, test once manually, and activate.
