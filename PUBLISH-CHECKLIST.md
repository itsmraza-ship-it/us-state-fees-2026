# Publish Checklist — us-state-fees-2026

**Nothing ships without Muhammad's explicit yes.**

- [ ] Muhammad approved this repo for public release (explicit yes)
- [ ] Copy `assets/epics-deals-ed-monogram.png` into `assets/` (referenced in README; image itself not included yet)
- [ ] Re-verify all 6 fees at the official state filing offices before publishing (fees change)
- [ ] Validate `fees.json` parses (`python3 -c "import json; json.load(open('fees.json'))"`) and matches `fees.csv`
- [ ] Decide GitHub org/name; after push add repo topics (`open-data`, `llc`, `startup`, `fintech`)
- [ ] Compliance spot-check passed: $130 + state fee only, no BOI-mandatory claims, no Pakistan mention, no guaranteed bank/Stripe approvals
