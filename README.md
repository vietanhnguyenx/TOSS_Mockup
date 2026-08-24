# TOSS — Interactive Mockups

UI mockups for the **TOSS** (Total Operations Steering System) project, published for review.

👉 **Open the mockups:** https://vietanhnguyenx.github.io/TOSS_Mockup/

## Available screens

| Screen | Module | Version | Link |
|---|---|---|---|
| Taxi Time | Data Maintenance › Airport Master Data | v1.4 | [taxi-time.html](https://vietanhnguyenx.github.io/TOSS_Mockup/taxi-time.html) |
| System Log | System Admin | v0.1 | [system-log.html](https://vietanhnguyenx.github.io/TOSS_Mockup/system-log.html) |
| Performance Factor | Operations Analysis | v0.15 | [performance-factor.html](https://vietanhnguyenx.github.io/TOSS_Mockup/performance-factor.html) |

## Performance Factor — what to look at

Three screens reached from the tabs at the top:

| Tab | What it does |
|---|---|
| **PF Messages From AC** | Which aircraft sent performance messages, and how many per flight. Export them to a text file, split by the tool that will process them |
| **Import Performance Data** | Load the result files produced by the manufacturer tools, review the validation preview, then write the data in |
| **PF Register** | Read the factor per aircraft, chart it over time, and list aircraft above a threshold. Export for OCD compares two months side by side |

Worth knowing while reviewing:

- The manufacturer tools run **outside** the system. This mockup covers the manual flow: export the
  messages, process them externally, bring the results back.
- **Colour means better or worse than baseline, not positive or negative.** A deviation and a factor
  always carry opposite signs, so a green row is green in every column.
- Out-of-range readings are removed in **two stages** — an absolute limit first, then a statistical one.
  Removed rows are still stored and shown, just left out of the average.
- **PF FMC is empty for the Boeing fleet.** The tool for that fleet does not output the fuel heating
  value needed to compute it. This is a real gap, not a missing screen.

## Notes

- These are **mockups, not a working system**. All airports, fleet groups, aircraft, values, users and
  timestamps are **sample data**; every action is simulated and nothing is saved.
- Layout and colours are a proposal, **pending BA/UI approval**.
- Self-contained HTML — no installation or download required, just open the link.
- Best viewed on a desktop browser at 1280 px width or wider.
