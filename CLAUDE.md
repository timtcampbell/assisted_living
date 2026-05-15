# Assisted Living Research Project

## Purpose

This project compares assisted living facilities in Wisconsin — primarily the greater Madison / Dane County area — to support an informed placement decision. Each facility gets its own markdown file. Reports must be consistent in structure so facilities can be compared side by side.

## Completed Facilities

| File | Facility | Location | Type |
|---|---|---|---|
| [beehive_mt_horeb.md](beehive_mt_horeb.md) | BeeHive Homes of Mt. Horeb | Mount Horeb, WI | CBRF — AL & Memory Care |
| [heritage_middleton.md](heritage_middleton.md) | Heritage Middleton | Middleton, WI | RCAC + CBRF — AL, Enhanced AL, Memory Care |
| [hatties_glen_waunakee.md](hatties_glen_waunakee.md) | Hattie's Glen Waunakee | Waunakee, WI | CBRF — AL & Memory Care |

---

## Report Template

Each report file must be named `{facility_slug}.md` (lowercase, underscores) and follow this exact section order.

---

### Header block (no section heading — appears at top of file)

```
# {Facility Full Name} — Research Summary

**Address:** {street}, {city}, WI {zip} | **Phone:** {phone}
**Operator:** {legal operator name}
**Wisconsin {license type} License:** {license number}
**Official website:** [{domain}]({url})
```

---

### 1. Facility Profile

Bullet list covering:
- **Type:** Wisconsin license type (CBRF / RCAC / AFH / etc.) and care categories offered
- **Capacity:** Number of units/beds and room types
- **Served populations:** Target resident groups (e.g., advanced aged, dementia/Alzheimer's)
- **Care levels offered:** List each level with a brief description (if multiple)
- **Staffing:** 24/7 coverage, whether a licensed nurse is on-site, notable staff ratios
- **Payment:** Private pay / Medicaid / Medicare / HCBS / VA benefits — be specific
- **Technology:** Any notable care or safety technology
- **Pricing:** Monthly cost range per care level; compare to area average

Use a pricing table when multiple care levels and room types exist.

---

### 2. Consumer Ratings — Aggregated Across Platforms

A markdown table with columns: Platform (linked), Score, # of Reviews.

Always check these platforms (fetch each, skip if 403/not found):
- A Place for Mom (aplaceformom.com)
- Caring.com
- Birdeye (birdeye.com)
- My Caring Plan (mycaringplan.com)
- Seniorly (seniorly.com)
- US News Best Senior Living (health.usnews.com)
- SeniorAdvisor (senioradvisor.com)
- LTC News (ltcnews.com)
- BBB (bbb.org)
- Yelp (yelp.com)

After the table, include:
- Statewide rank if available (My Caring Plan or US News)
- Parent-company average if the facility is part of a chain

#### Sub-sections (include only when data is available):

**A Place for Mom Category Ratings** — table of per-category scores (Cleanliness, Friendliness, Care Services, Staff, Meals & Dining, Activities, Value for Cost)

**Caring.com Category Ratings** — table if available (Facility, Staff, Food, Activities, Value)

**A Place for Mom Rating Distribution** — 5-star through 1-star breakdown as percentages and counts

**Awards Earned** — any Best of Senior Living, Most Friendly, etc.

---

### 3. What Reviewers Say

Three subsections:

**Positives consistently cited:** Bullet list of themes that appear across multiple reviews.

**Notable positive quotes:** Italicized verbatim quotes with source attribution and date where known.

**Concerns and criticisms:** Bullet list of recurring negative themes, bolded by topic (e.g., **Staffing**, **Food quality**).

**Notable critical quotes:** Italicized verbatim quotes with source attribution and date where known.

If no negative reviews exist, state that explicitly and note the low review volume caveat.

---

### 4. Employee Satisfaction

Source the data (typically My Caring Plan or Glassdoor). Include:
- Overall employee rating and grade
- Sub-scores: pay, staff environment
- Qualitative themes from employee reviews
- Note whether the data is facility-specific or chain-wide

---

### 5. State Regulatory / Inspection Data

Always include:
- **Licensed by:** Wisconsin DHS, Division of Quality Assurance — include license number and type
- **HCBS compliant:** Yes / No (determines Medicaid waiver eligibility)
- **Inspections:** Summary of any found violations, deficiencies, or citations. If none found, state so explicitly and direct the reader to:
  - [ForwardHealth DQA Provider Search](https://www.forwardhealth.wi.gov/WIPortal/Subsystem/Public/DQAProviderSearch.aspx)
  - Email: dhswebmaildqa@dhs.wisconsin.gov
- **CMS Care Compare visibility:** Note whether Medicare/Medicaid acceptance makes the facility visible in federal databases
- **WALA membership:** Check [ewala.org](https://www.ewala.org) provider search

To look up a facility's Wisconsin license number, search:
- CBRF facilities: `https://www.forwardhealth.wi.gov/WIPortal/Subsystem/Public/DqaProviderSearchResults.aspx?fac_type=cbrf&county={county}`
- RCAC facilities: `https://www.forwardhealth.wi.gov/WIPortal/Subsystem/Public/DqaProviderSearchResults.aspx?fac_type=rcac&county={county}`
- Dane County is the correct county for Madison-area facilities

---

### 6. Bottom Line

Two to four sentences. Cover:
1. What the facility does well (type of resident it suits best)
2. Key weaknesses or caveats
3. One concrete action item for families (what to ask or verify during a tour / what record to request)

---

### 7. Sources

Bulleted list of all sources consulted, each as a labeled markdown link. Include even sources that returned 403 or no data, so the next researcher knows what was tried.

---

### Footer

```
---

*Researched {Month DD, YYYY}*
```

---

## Research Approach

Run these steps for each new facility:

1. **Parallel initial searches** — run three WebSearch queries simultaneously:
   - `{facility name} assisted living Wisconsin reviews`
   - `{facility name} assisted living quality ratings scores Wisconsin`
   - `"{facility name}" assisted living inspection violations Wisconsin DHS`

2. **Parallel page fetches** — fetch A Place for Mom, Caring.com, Birdeye, US News, and My Caring Plan simultaneously. US News often times out; retry once.

3. **Find the Wisconsin license number** — search the ForwardHealth DQA provider list for the appropriate county and care type. Record the license ID; use it to look up any available survey/inspection history.

4. **Fetch the official facility website** — extract care types, staffing, pricing, and payment details.

5. **Check WALA membership** — search ewala.org provider directory.

6. **Fill gaps** — run follow-up searches for any sections still missing data (e.g., employee reviews, Google rating, BBB complaints).

7. **Write the file** using the template above. Cross-reference other completed reports in the Bottom Line where useful for comparison.

---

## Wisconsin License Types

| Abbreviation | Full Name | Typical Size | Medicaid |
|---|---|---|---|
| CBRF | Community-Based Residential Facility | 5–20 beds (small) | Sometimes |
| RCAC | Residential Care Apartment Complex | Larger, apartment-style | Sometimes (HCBS) |
| AFH | Adult Family Home | 1–4 residents | Often |
| NH | Nursing Home | Skilled nursing | Yes (Medicare/Medicaid) |

---

## Key Reference Links

- [Wisconsin DHS ForwardHealth DQA Provider Search](https://www.forwardhealth.wi.gov/WIPortal/Subsystem/Public/DQAProviderSearch.aspx)
- [Wisconsin DHS Consumer Guide — Finding an Assisted Living Facility](https://www.dhs.wisconsin.gov/guide/assisted-living.htm)
- [Wisconsin Assisted Living Association (WALA) Provider Search](https://www.ewala.org/provider-search)
- [Dane County ADRC — DQA Survey History Guide (PDF)](https://daneadrc.org/documents/pdf/Resources/Housing/ALF-DQA-Survey-History-Search.pdf)
- DQA inspection record requests: dhswebmaildqa@dhs.wisconsin.gov
