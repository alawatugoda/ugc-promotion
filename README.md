# UGC Promotion Self-Assessment Tool

A self-evaluation tool for **UGC Merit Promotion** (Associate Professor / Professor), based on **Commission Circular No. 916 (2009)**.

## What it does

- Fetches your publications automatically from [OpenAlex](https://openalex.org/) using your Author ID
- Scores §2.1.1 journal papers (frequency + WoS indexing + joint authorship contribution)
- Scores §2.1.2 conference papers (full paper / abstract / presented)
- Manual entry for citations (§2.1.3) and all other sections (§1, §2, §3)
- Checks eligibility against minimum marks for each post type
- Generates a print-ready summary report

## Files

| File | Description |
|---|---|
| `ugc_promotion.html` | Main tool — open in any browser |
| `scimago_issn.json` | Scimago 2025 journal rankings (ISSN → Quartile) |

> **Both files must be in the same folder** for WoS/quartile detection to work.

## How to use

1. Open `ugc_promotion.html` in your browser
2. Fill in your personal details and select the post you are applying for
3. Enter your **OpenAlex Author ID** and click **Fetch Publications**
4. Review and adjust journal frequency and WoS status for each paper
5. Enter citation count (§2.1.3) and fill in all other sections manually
6. Click **🖨️ Print / PDF** to generate the summary report
7. Use **💾 Save JSON** to save your progress; **📂 Load JSON** to restore it

## Scoring Summary (Circular No. 916)

### §2.1.1 — Journal Publications
| Frequency | Base pts | WoS indexed |
|---|---|---|
| ≥ 2 issues/year | 3 pts | +2 pts |
| < 2 issues/year | 2 pts | +2 pts |

Adjust for joint authorship using the **Contribution %** field.

### §2.1.2 — Conference Presentations
| Type | Points | Cap |
|---|---|---|
| Full paper published | up to 1 pt | Max 15 |
| Abstract published | up to 0.75 pt | Max 5 |
| Presented with evidence | up to 0.5 pt | Max 5 |

### §2.1.3 — Citations
0.5 pt per citation. Attach Google Scholar or Scopus PDF as evidence.

## Minimum Marks

| Post | §1 Teaching | §2 Research | §2.1.1 Journals | §3 University | Total |
|---|---|---|---|---|---|
| Associate Prof (Internal) | 10 | 25 | 12 | 10 | 70 |
| Associate Prof (External) | 5 | 35 | 12 | 5 | 70 |
| Professor (Merit) | 20 | 50 | 12 | 10 | 105 |
| Professor (Cadre) | 25 | 55 | 12 | 15 | 115 |

## Saving your data

Use **💾 Save JSON** to export your data. Use **📂 Load JSON** to restore it. Data is **not** saved in the browser — always save before closing.

## Live version

**[https://alawatugoda.github.io/ugc-promotion/ugc_promotion.html](https://alawatugoda.github.io/ugc-promotion/ugc_promotion.html)**

---

*Based on UGC Commission Circular No. 916 (2009).*
