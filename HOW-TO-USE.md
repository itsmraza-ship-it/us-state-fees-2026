# How to Use This Repo

**US State Fees 2026** — open data on what each US state charges to
form an LLC (state filing fee only). Free for calculators,
comparison tools, dashboards, and guides.

Pick the route that fits how you work:

## 1. As a Claude skill

1. Copy this repo's `SKILL.md` into your Claude skills folder (or
   upload it wherever your setup accepts skills).
2. Ask in this repo's domain, e.g. "What's the LLC filing fee in
   Florida?" — Claude answers from the verified table ($125,
   verified Oct 2026) and flags unverified states as "varies".

## 2. Inside Claude.ai

1. Create a Project in Claude.ai.
2. Paste `SKILL.md` into the Project's instructions, and/or add
   `SKILL.md`, `fees.csv`, and `fees.json` as Project knowledge.
3. Ask fee and state-comparison questions inside that Project.

## 3. With the Epics Deals MCP server (live answers)

These are static knowledge files. For live tool answers instead,
connect the Epics Deals MCP server:

- Endpoint: `https://epics-deals-mcp.epicsdeals.workers.dev/mcp`
- Add it as a remote MCP server in your AI client, then ask your
  fee questions — the tools answer live instead of from static files.

## 4. As plain reference / data download

1. Read `README.md` on GitHub for the verified values and coverage.
2. Download `fees.csv` for spreadsheets and quick analysis.
3. Download `fees.json` for apps, APIs, and static sites — see the
   Python and JavaScript snippets in the README.
4. Check `CHANGELOG.md` before relying on a figure; fees change, so
   confirm at the state's filing office before filing.

## 5. In other AI tools

1. Upload `SKILL.md` plus `fees.csv` / `fees.json` as knowledge to a
   custom GPT, a Gemini Gem, or a notebook.
2. Ask fee questions — the model should quote only verified states
   and say "varies — check the state's filing office" for the rest.

## 6. Fork it

This repo is MIT licensed. Fork it and build your own calculator or
comparison tool on the data. Found a changed fee? PR `fees.csv`,
`fees.json`, and `CHANGELOG.md` with the official state source.

---

epicsdeals.com — free tools by Epics Deals; US LLC formation from $130 + state fee.
