# Topic status

Companion continuity record for the stable IDs in Engineering_Knowledge_Hub_Project_Pack.md. Repository and PR state remain authoritative. Merged does not establish published.

| ID | State | Branch / file | Evidence | Last checked |
| --- | --- | --- | --- | --- |
| DD-20 | Merged | content/dd-20-ai-code-evidence / ai-code-evidence.html | Article and index integrated. DOM logic and structural checks passed; browser visual and keyboard checks blocked. [Merged PR #3](https://github.com/shawshannk/engineering-articles/pull/3). | 2026-10-12 |

## EX-07 brief

- State: Draft; branch content/ex-07-hidden-queries; page hidden-queries.html; PR pending. Not merged or published.
- Outcome: distinguish HTTP calls from database round trips and identify query-count growth with page size.
- Assumptions: stable relational data, exactly 10/50/100 orders, required tenant-consistent customer reference, explicit per-order query with no cache/batch, simple joined projection, no failures/retries/extra count queries. Reads are not modeled inside a transaction.
- Interactions: seven meaningful phases, grouped lookup visualization, page size and strategy controls, Play/Pause/Next/Replay. Counters distinguish HTTP requests, database statements and delivered response rows; progress tracks rows assembled at the API.
- Verification: actual page script executed in jsdom across six combinations and every transition/counter; autoplay completion, manual next, pause/resume remaining delay and animation API calls, both setting resets, replay, visibility/pagehide pause, reduced motion including mid-flow changes, JS-disabled fallback. Static IDs, anchors, local links, no-em-dash rule and diff whitespace checked.
- Limitations: Chromium absent. DOM checks and animation stubs do not establish real desktop/mobile layout, keyboard behavior or browser animation. No database or C# application executed. Code excerpts are labeled illustrative.
- Sources: Microsoft EF Core efficient querying and lazy-loading documentation. Existing TB-01 linked at n-plus-one.html.
- Caption: One request in the browser can become 101 queries in the database. Watch where the extra calls come from.

## EX-19 brief

- State: Merged; branch content/ex-19-refresh-reuse; page refresh-token-reuse.html. [Merged PR #4](https://github.com/shawshannk/engineering-articles/pull/4). Confirmed on main 2026-10-13; deployment not verified.
- Outcome: follow token rotation and distinguish strict reuse detection from a documented provider-specific reuse interval.
- Assumptions: bearer refresh tokens, one tracked family, atomic serialized server updates, Tab A wins, ordered responses, no further refreshes; +1/+8 seconds and 5-second interval are illustrative.
- Policy: strict family revocation versus Auth0-style overlap issuing another successor. Early thief and legitimate tab receive the same policy outcome. No claim that every provider behaves this way.
- Checks: actual page script executed in jsdom for all six combinations and 30 transitions; final token states/counts, manual next, autoplay completion, pause/resume remaining delay and animation API calls, replay, scenario reset, hidden-page/pagehide pause, reduced motion, no-JS fallback. Static IDs/local links and diff whitespace checked.
- Limits: Chromium unavailable. DOM/animation stubs do not verify real rendering, keyboard behavior, responsive layout or browser animation. No real authentication server tested.
- Sources: RFC 9700 section 4.14.2 and current Auth0 rotation/overlap documentation, linked in page.
- Team caption: Two requests. One refresh token. See why the same reuse policy can tolerate a second tab and admit an early replay.

## DD-20 brief

- Format: 5–10 minute deep dive, approximately 8 minutes.
- Outcome: connect an AI-generated change to scoped, inspectable verification evidence and a reviewable handoff.
- Example assumptions: ASP.NET Core, System.Text.Json, existing relational column, known consumers, tenant-restricted order endpoint; field always present, string or explicit null. No new persistence operation or transaction is introduced.
- Acceptance: readable standalone HTML; existing paper/orange styling; populated/null JSON comparison; meaningful verification limits; low/moderate/high planning aid; handoff comparison and reusable template; valid local navigation and index entry; no claims of executed example API tests.
- Sources: Microsoft System.Text.Json property omission and ASP.NET Core integration testing documentation, linked in the article.
- Logic verification: actual page script executed in jsdom. All three risk plans, every checkbox on/off, progress counts, clearing on plan changes, reset to moderate, input labels, no script errors, and JS-disabled fallback checked.
- Structural verification: unique static IDs, internal anchors, local file links, no em dashes in new page, diff whitespace, existing article preservation. No new runtime dependencies.
- Limitations: Chromium was absent and its download failed. Desktop/mobile rendering, native details interaction, keyboard focus, and reduced-motion behavior have not been browser-verified. Page has no animation; reduced-motion CSS disables smooth scrolling. C# snippets and fictional command results are explicitly illustrative, not compiled or run against an API project.
- Current repository evidence: PR #3 merged into main; deployment not verified.

Optional team-sharing caption: AI can write the code. What evidence makes the change reviewable? A practical deep dive with an API example, a risk-based checklist, and a reusable handoff.
