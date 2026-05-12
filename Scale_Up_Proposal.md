
# 1000-Company Scale-Up Proposal

## Objective: Build a list of 1000 ICP-qualified companies in 30 days.

## Week-by-Week Plan

### Week 1: Bulk Universe Building
- **Sourcing**: Use Python scrapers (Selenium/Scrapy) to pull data from:
    - **Indiamart/Kompass**: Targeted at 'Manufacturers' in Specialty Chemicals, MedTech, and Biotech.
    - **MSME Data**: Export lists of Pune/Ahmedabad/Hyderabad companies with 'Specialty' or 'Technical' tags.
    - **Patent Databases**: Pull names of companies filing patents in India over the last 3 years.
- **Output**: 5,000 raw leads.

### Week 2: AI-Powered Qualification
- **Automation**: Use an LLM (Claude/GPT-4) via API to scan company websites.
- **Prompt Logic**: "Analyze this company website. Is it a manufacturer? Does it have a technical founder? Score it against these 6 criteria..."
- **Disqualification**: Auto-filter for keywords like 'Distributor', 'Trader', 'CRO', 'Service Provider'.
- **Output**: 1,500 scored candidates.

### Week 3: Deep Verification & Revenue QC
- **Data Enrichment**: Run the 1,500 candidates through a Tofler/Zauba API to get precise revenue and ownership data (PE-owned check).
- **Human-in-the-loop**: Manually audit the top 20% to verify the 'Technical DM' and 'Growth Hook' quality.
- **Output**: 1,100 verified candidates.

### Week 4: Personalization & Delivery
- **Hook Generation**: Use AI to draft the 'Personalization Hook' based on recent news or specific product USPs found during the scrape.
- **Final Scrub**: Remove duplicates and subsidiaries of large groups.
- **Output**: 1,000 Final Federated Targets.

## Expected Yield & Quality Control
- **Initial Raw List**: 5,000
- **AI Qualified**: 1,500 (30% yield)
- **Revenue/Owner Qualified**: 1,000 (66% yield from the 1,500)
- **QC**: 5% random sampling every day to ensure the AI scoring isn't hallucinating.
