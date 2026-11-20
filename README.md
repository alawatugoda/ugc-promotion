# UGC Promotion Self-Assessment Tool

A browser-based self-evaluation tool for **UGC Merit Promotion** (Associate Professor / Professor), based on **Commission Circular No. 916 — 30 September 2009**.

> **No installation. No server. Open `ugc_promotion.html` in any browser and start.**

---

## 🔗 Live Version

**[https://alawatugoda.github.io/ugc-promotion/ugc_promotion.html](https://alawatugoda.github.io/ugc-promotion/ugc_promotion.html)**

---

## Features

### Automatic Publication Fetching
- Fetches your publications from [OpenAlex](https://openalex.org/) using your Author ID
- Auto-detects journal frequency (≥2/yr or <2/yr) and WoS indexing
- Checks [Scimago Journal Rankings](https://www.scimagojr.com/) for quartile (Q1–Q4)
- Duplicate detection when adding papers manually via DOI
- Move papers between sections (Journals ↔ Conference ↔ Books)

### Scoring (Circular No. 916)
- **§1** Teaching, Scholarship & Academic Development — full manual entry with date-based calculation
- **§2.1.1** Journal publications — frequency + WoS + contribution %
- **§2.1.2** Conference papers — full / abstract / presented with contribution %
- **§2.1.3** Citations — per-paper or bulk entry with 0.5 pt/citation (max 10 per work)
- **§2.2–§2.4** Scholarly work, creative work, patents
- **§3** Contributions to University & National/International Development
- Caps and eligibility checks per post type

### Evidence Management
- Attach PDF evidence to every entry
- Save evidence files to a local folder with auto-generated reference numbers (e.g. `2.1.1.01`)
- Re-link evidence from folder on JSON reload
- Reference numbers shown in print report

### Print & PDF
| Button | Output |
|---|---|
| 🖨️ **Print Assessment** | Marking scheme + evidence detail tables (fast, no PDFs) |
| 📄 **Print §1** | §1 Teaching evidence PDFs only |
| 📄 **Print §2** | §2 Research evidence PDFs only |
| 📄 **Print §3** | §3 Contributions evidence PDFs only |

Each section print includes a cover page, sub-section dividers, and reference-numbered PDF pages.

### Other
- Dark / light theme toggle
- Save progress as JSON — restore anytime with Load JSON
- Score tiles with eligibility indicator per section
- Works fully offline (no server, no login)

---

## Files

| File | Description |
|---|---|
| `ugc_promotion.html` | Main tool — open in any modern browser |
| `scimago_issn.json` | Scimago 2025 journal rankings (ISSN → Quartile) |
| `scimagojr 2025.csv` | Source CSV for the above |

> **Both `ugc_promotion.html` and `scimago_issn.json` must be in the same folder** for WoS/quartile detection to work.

---

## How to Use

1. Download `ugc_promotion.html` and `scimago_issn.json` to the same folder
2. Open `ugc_promotion.html` in Chrome or Edge (Firefox also works)
3. Fill in your personal details and select the post you are applying for
4. Enter your **OpenAlex Author ID** and click **Fetch Publications**
5. Review journal frequency and WoS status for each paper; adjust contribution %
6. Fill in all other sections manually (§1, §2.2–§2.4, §2.1.3 citations, §3)
7. Attach PDF evidence to each entry using the 📎 button
8. Click **💾 Save** to save progress and write evidence PDFs to a folder
9. Click **🖨️ Print Assessment** for the marking scheme report
10. Click **📄 Print §1 / §2 / §3** to print evidence PDFs by section

---

## Scoring Summary (Circular No. 916)

### §2.1.1 — Journal Publications
| Frequency | Base pts | + WoS indexed |
|---|---|---|
| ≥ 2 issues/year | 3 pts | +2 pts |
| < 2 issues/year | 2 pts | +2 pts |

Multiply by **Contribution %** for joint-authored papers.

### §2.1.2 — Conference Papers
| Type | Points | Cap |
|---|---|---|
| Full paper published | up to 1 pt | Max 15 pts |
| Abstract published | up to 0.75 pt | Max 5 pts |
| Presented with evidence | up to 0.5 pt | Max 5 pts |

### §2.1.3 — Citations
0.5 pt per citation, max 10 pts for repeated citations of the same work.

---

## Minimum Marks for Eligibility

| Post | §1 Teaching | §2 Research | §2.1.1 Journals | §3 University | Total |
|---|---|---|---|---|---|
| Associate Professor (Internal) | 10 | 25 | 12 | 10 | 70 |
| Associate Professor (External) | 5 | 35 | 12 | 5 | 70 |
| Professor (Merit) | 20 | 50 | 12 | 10 | 105 |
| Professor (Cadre) | 25 | 55 | 12 | 15 | 115 |

---

## Powered by Open Data

- [OpenAlex](https://openalex.org/) — publication and citation data (free, open)
- [Scimago Journal Rankings](https://www.scimagojr.com/) — journal quartile data

---

## Developer

**Dr. Janaka Alawatugoda**

- BSc (Hons) Computer Science — University of Peradeniya
- PhD — Queensland University of Technology, Australia
- Fellow, British Computer Society (FBCS)
- Senior Member, Association for Computing Machinery (SMACM)
- Member, Computer Society of Sri Lanka

🔗 [LinkedIn](https://www.linkedin.com/in/alawatugoda-phd-fbcs-smacm-mcs-sl-53294034/) &nbsp;·&nbsp; ✉️ alawatugoda@eng.pdn.ac.lk

---

*Based on UGC Commission Circular No. 916 — 30 September 2009.*
