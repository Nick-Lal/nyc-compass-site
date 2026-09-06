# NYC Compass — site

The published static site for **NYC Compass**: from one New York City address, what you can build
there and what government funding may apply.

**Live:** https://nick-lal.github.io/nyc-compass-site/

## What is here, and what is not

This repository holds only the published site — two HTML pages and one JSON data file. It is
generated; **do not edit it here.** The source, the tests, and the research notes live in a separate
private repository, and this tree is pushed from there.

| File | What it is |
|---|---|
| `funding.html` | The funding directory. Fully working — 37 programmes, filterable, each cited |
| `index.html` | The address lookup. Explains itself and links to the directory, because the lookup needs a server that is not running here |
| `data/programs.json` | The programmes, generated from the source repository |

## What works on a static host, and what does not

The **funding directory works completely.** It reads one JSON file and filters in the browser.

The **address lookup does not**, and says so plainly rather than failing vaguely. Geocoding, the
PLUTO parcel record, and the point-in-polygon test against incentive-area boundaries all happen
server-side, and there is no server here. That page invites you to the directory instead.

## Honesty

This is an independent prototype built from public data. It is **not** an official service of,
affiliated with, or endorsed by the City of New York, New York State, or the State of Maryland. It
shows *potential* eligibility only and is not legal, financial, or land-use advice. Every answer
cites its source and the date that source was last checked.

Every programme shown has been checked against its official page by a person, and an automated
check re-verifies those citations — 100% of the 35 machine-checkable records currently have nothing
contradicting them. One programme was **removed** from this site because its official page went
offline and no replacement could be found: a record that cannot be cited does not belong on a page
whose promise is citation.

Built by Nick Lal with [Claude Code](https://claude.com/claude-code). Inspired by the
[Maryland Community Compass](https://compass.maryland.gov/) and its public MCP server, built by the
Maryland State Innovation Team.
