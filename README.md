# NYC Compass — site (retired copy)

**The site moved on 2026-10-10** to **https://nyc-compass.nicholas-ravi-lal.workers.dev/**, where one Cloudflare
Worker serves the pages and the Model Context Protocol (MCP) endpoint together, so the address lookup works there and
the pages can never show different data from the tools. The source, the tests and the research notes live in the
private `nyc-compass` repository; the move is explained in its `research/35-cloudflare-static-assets.md`.

This repository held the GitHub Pages build of the site from 2026-08 to 2026-10-10 (two pages and one data file,
pushed from the source repository). It now holds only redirect pages: `index.html`, `funding.html` and `map.html` send
visitors to the same page on the new address, `404.html` sends everything else to the home page, and `robots.txt`
asks crawlers to leave this copy alone. Nothing here is edited by hand except this retirement.

NYC Compass is an independent prototype built from public data. It is **not** an official service of, affiliated
with, or endorsed by the City of New York, New York State, or the State of Maryland. It shows *potential* eligibility
only and is not legal, financial, or land-use advice.

Built by Nick Lal with [Claude Code](https://claude.com/claude-code). Inspired by the
[Maryland Community Compass](https://compass.maryland.gov/) and its public MCP server, built by the Maryland State
Innovation Team.
