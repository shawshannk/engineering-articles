# Topic status

Companion continuity record for the stable IDs in Engineering_Knowledge_Hub_Project_Pack.md. Repository and PR state remain authoritative. Merged does not establish published.

| ID | State | Branch / file | Evidence | Last checked |
| --- | --- | --- | --- | --- |
| DD-20 | PR open (draft) | content/dd-20-ai-code-evidence / ai-code-evidence.html | Article and index integrated. DOM logic and structural checks passed; browser visual and keyboard checks blocked. [Draft PR #3](https://github.com/shawshannk/engineering-articles/pull/3). | 2026-10-12 |

## DD-20 brief

- Format: 5–10 minute deep dive, approximately 8 minutes.
- Outcome: connect an AI-generated change to scoped, inspectable verification evidence and a reviewable handoff.
- Example assumptions: ASP.NET Core, System.Text.Json, existing relational column, known consumers, tenant-restricted order endpoint; field always present, string or explicit null. No new persistence operation or transaction is introduced.
- Acceptance: readable standalone HTML; existing paper/orange styling; populated/null JSON comparison; meaningful verification limits; low/moderate/high planning aid; handoff comparison and reusable template; valid local navigation and index entry; no claims of executed example API tests.
- Sources: Microsoft System.Text.Json property omission and ASP.NET Core integration testing documentation, linked in the article.
- Logic verification: actual page script executed in jsdom. All three risk plans, every checkbox on/off, progress counts, clearing on plan changes, reset to moderate, input labels, no script errors, and JS-disabled fallback checked.
- Structural verification: unique static IDs, internal anchors, local file links, no em dashes in new page, diff whitespace, existing article preservation. No new runtime dependencies.
- Limitations: Chromium was absent and its download failed. Desktop/mobile rendering, native details interaction, keyboard focus, and reduced-motion behavior have not been browser-verified. Page has no animation; reduced-motion CSS disables smooth scrolling. C# snippets and fictional command results are explicitly illustrative, not compiled or run against an API project.
- Merge and deployment: not authorized or performed.

Optional team-sharing caption: AI can write the code. What evidence makes the change reviewable? A practical deep dive with an API example, a risk-based checklist, and a reusable handoff.
