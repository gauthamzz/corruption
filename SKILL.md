# Build a Corruption Dashboard for Your Country

Send this entire file to your AI agent (Claude, ChatGPT, etc.) and tell it your country name. It will build a complete corruption dashboard.

Repository: https://github.com/gauthamzz/corruption
Reference: https://gauthamzz.github.io/corruption (India's live version)

---

## Prompt for AI Agent

You are building a **corruption dashboard** — a single-page interactive website that shows citizens of **[COUNTRY]** where their tax money goes and how much is lost to corruption, leakage, and inefficiency.

Use the India version as a reference for design and structure: https://github.com/gauthamzz/corruption

### What to Build

A single `index.html` file. No frameworks, no build step, no dependencies beyond Google Fonts. Dark theme using the country's flag colors as accents.

### Sections Required

#### 1. Hero
- Country name, flag colors as accent bar
- Title in local language + English: "How Much of Your Life Did Corruption Eat?"
- Subtitle explaining the dashboard

#### 2. Personal Tax Calculator
- Inputs: Region/State/Province, Monthly Income (local currency), Monthly Spending, Age
- Calculate:
  - Annual tax paid (income tax + consumption tax like VAT/GST/sales tax)
  - Estimated amount lost to corruption/leakage (use the country's known leakage rate from audits)
  - Convert to **working days lost per year** (annual corruption loss / daily income)
  - Lifetime loss until retirement
- Show results in a big card with breakdown stats

#### 3. Getting Worse — What Audits Found
- Find **6-8 recent audit findings** from the country's Supreme Audit Institution (SAI)
- Each card needs: title, big stat number, 1-2 line description, source attribution
- Use real numbers from real audits. No opinions. Examples of what to look for:
  - Ghost beneficiaries in welfare programs
  - Cost overruns in infrastructure
  - Fraud in healthcare/education schemes
  - Tax collection irregularities
  - Public procurement fraud

#### 4. Getting Better — What's Actually Improving
- Find **6-8 measurable improvements**. Every country has some. Be fair and balanced.
- Examples: digitization reducing leakage, transparency portals, audit reforms, anti-corruption convictions
- Same card format: title, stat, description, source

#### 5. Region/State Comparison
- Cards for each major region/state/province showing:
  - Share of national tax received (%)
  - Value multiplier (regional GDP / central transfers)
  - Public service leakage rate (%)
  - Governance quality rating
  - Visual leak bar (% kept vs % leaked)
- Tabs: Overview, Biggest Takers, Value Creators
- Highlight user's selected region with a "You" tag

#### 6. Corruption Perceptions Index Chart
- Bar chart showing the country's CPI score from Transparency International (2012-2025)
- Dashed line for global average (~43)
- Data: https://www.transparency.org/cpi

#### 7. Call to Action
- Goal: reduce corruption days to 0
- Action chips: file information requests (RTI/FOIA equivalent), track spending, read audits
- Share buttons: Twitter/X, WhatsApp, copy text

#### 8. Movement Section
- "This was built by talking to AI. Anyone can build one for their country."
- Show which countries have dashboards (India = live, others = wanted)
- Link to this repo

#### 9. Sources Section
- Grid of every data source used
- Each source: icon, name, description, link
- Every number in the dashboard must trace back to a source here

### Where to Find Data

| Data | Source |
|------|--------|
| Government audit findings | Country's Supreme Audit Institution (SAI) |
| Corruption perception score | Transparency International CPI |
| Tax structure & rates | Ministry of Finance / Revenue Authority |
| Budget & spending data | National budget documents, World Bank BOOST |
| Service delivery leakage | World Bank surveys, national household surveys |
| Regional fiscal data | Finance commission, statistical office, central bank |
| Welfare efficiency | UNDP, World Bank governance indicators |

### Supreme Audit Institutions by Country

| Country | SAI | Website |
|---------|-----|---------|
| India | CAG | cag.gov.in |
| USA | GAO | gao.gov |
| UK | NAO | nao.org.uk |
| Brazil | TCU | tcu.gov.br |
| Nigeria | OAuGF | oaugf.ng |
| Indonesia | BPK | bpk.go.id |
| Philippines | COA | coa.gov.ph |
| Mexico | ASF | asf.gob.mx |
| South Africa | AGSA | agsa.co.za |
| Kenya | OAG | oagkenya.go.ke |
| Bangladesh | OCAG | cagbd.org |
| Pakistan | AGP | agp.gov.pk |
| Germany | BRH | bundesrechnungshof.de |
| France | Cour des comptes | ccomptes.fr |
| Japan | BAJ | jbaudit.go.jp |
| Australia | ANAO | anao.gov.au |
| Canada | OAG | oag-bvg.gc.ca |

If your country isn't listed, search "[country name] supreme audit institution" — every country has one.

### Design Rules

- **Dark theme**: Background #06060a, surfaces #0d0d14 / #14141f
- **Flag colors**: Use 2-3 colors from the country's flag as accents (saffron/green for India, green/yellow for Brazil, etc.)
- **Fonts**: Instrument Serif (headings), Outfit (body), IBM Plex Mono (numbers). Add the country's script font if applicable (e.g., Noto Sans Devanagari for Hindi)
- **Mobile responsive**: Must work on phones. Use clamp() for font sizes, grid with auto-fit
- **No tracking**: No cookies, no analytics, no data stored
- **Single file**: Everything in one index.html — CSS in `<style>`, JS in `<script>`

### Tone

- Non-partisan. No party politics. Criticize systems, not parties.
- Data-driven. Every claim has a source.
- Balanced. Show what's broken AND what's improving.
- Angry but constructive. The goal is accountability, not despair.

---

## How to Use This Skill

1. Copy this entire file
2. Send it to your AI agent
3. Tell it: "Build this for [YOUR COUNTRY]"
4. The AI will research your country's audit data and generate a complete `index.html`
5. Host it anywhere (GitHub Pages, Vercel, Netlify, or just open the file)
6. Submit a PR to https://github.com/gauthamzz/corruption

## License

Public domain. The data is public. The code is free. The anger is universal.
