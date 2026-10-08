# Best Workplaces Insights page: redesign mockup

Redesign and copy rewrite of https://greatplacetowork.com.au/reports/best-workplaces-insights/.
Open `index.html` in a browser. Highlighted values are unverified.

## Before go-live (blocking)

- [ ] Verify **128,405** respondents and **92.5% vs 49.6%** ("management does what it says") against the published 2026 report. These came from public summaries, not the report itself.
- [ ] Fill every `[XX]` stat and `[Finding 4]` from the report. Never ship a placeholder or an estimate.
- [ ] Define the "typical Australian workplace" comparison sample in the source line. ACCC substantiation applies.
- [ ] Confirm "pride was the strongest indicator of retention" is stated in the 2026 report.
- [ ] Wire the form to the existing HubSpot form and the PDF delivery email. The email must deliver exactly what the form promises.
- [ ] Replace the placeholder cover with the real report cover, and add real library links.

## Page structure and why

1. **Hero:** names the report and the dataset, with one primary CTA. Leads with provenance (employee responses), not aspiration.
2. **Stats strip:** shows the gap, with the source visible on the page.
3. **Inside the report:** findings stated up front instead of a table of contents.
4. **How People leaders use it:** gives the HR proposer an argument for their board.
5. **Method:** "Decided by employees, not a judging panel."
6. **Form:** six fields; company size routes the sales conversation; delivery expectation stated.
7. **Report library:** gives returning visitors more reports to read.
8. **Bridge CTA:** one low-pressure link to the Trust Index™ (Culture Intelligence). No Certification CTA, so the page stays on one pillar.

## Replicating for other markets

Every market-specific value carries `data-market="..."` in the HTML. Swap these tokens:

| Token | AU value | Notes |
|---|---|---|
| `list-name` | Best Workplaces™ in Australia | Use the market's official list name |
| `year` | 2026 | Appears in the eyebrow, cover, source line and form heading |
| `respondents` | 128,405 | Market sample only, never a regional total |
| Stats ×3 | 92.5% / 49.6% etc. | Must come from that market's report, with that market's source line |
| H1 country | "Australia's" | Also in the stats "vs typical [country] workplaces" |
| Library cards | AU reports | Use only reports that exist in that market |
| Spelling | AU | SG/NZ use UK/AU spelling; PH uses US spelling |

Market rules:
- Do not carry AU figures into another market's page, and do not mix 15x and 10x attraction stats in one funnel.
- Check each market's context and claim-check rules (SG has its own restricted-claims register) before publishing.
