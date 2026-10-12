# US State Fees 2026 — LLC Formation Filing Fees

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Verified: Oct 2026](https://img.shields.io/badge/Verified-Oct%202026-black)
![Format: CSV + JSON](https://img.shields.io/badge/Format-CSV%20%2B%20JSON-brightgreen)

Open data: **what each US state charges to form an LLC** (state filing fee only — not service fees). Free for developers to use in calculators, comparison tools, dashboards, and guides.

## The data

| File | Use it for |
|------|-----------|
| [`fees.csv`](fees.csv) | Spreadsheets, quick analysis |
| [`fees.json`](fees.json) | Apps, APIs, static sites — machine-readable |

Columns: `state` · `filing_fee_usd` · `verified_source_note` · `disclaimer`

**Current values (verified Oct 2026):** Wyoming $102 · New Mexico $50 · Delaware $90 · Missouri $50 · Texas $308 · Florida $125.

## Quick start

```python
import json, csv

# JSON
with open("fees.json") as f:
    data = json.load(f)
    for row in data["fees"]:
        print(row["state"], row["filing_fee_usd"])

# CSV
with open("fees.csv") as f:
    for row in csv.DictReader(f):
        print(row["state"], row["filing_fee_usd"])
```

```js
// JavaScript
const data = await (await fetch("fees.json")).json();
console.table(data.fees);
```

## Coverage & accuracy

- **6 states verified** (the most popular with non-resident founders). Other states: fees **vary** — check the state's filing office; we don't publish fees we haven't verified.
- **Formation filing fees only.** Annual reports, franchise taxes, and expedited fees are separate.
- **Fees change.** Last verified October 2026 — see [CHANGELOG.md](CHANGELOG.md). Always confirm at the state's filing office before filing.

## Contributing

State raised (or lowered) a fee? Open a PR updating `fees.csv`, `fees.json`, and [CHANGELOG.md](CHANGELOG.md) — with the official state source linked.

## Who maintains this

[Epics Deals](https://epicsdeals.com) — US company formation for founders worldwide. Formation **$130 + state fee** · [WhatsApp](https://wa.link/x6klxo) · [info@epicsdeals.com](mailto:info@epicsdeals.com)

---

<p align="center">
  <strong>Your next big deal starts here.</strong>
</p>
