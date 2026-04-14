# Web Research Guidelines for Selma

## 0. Reasoning Before Search (Georg's Feedback)
- **Always reason first** before issuing a search. Ask: *Can I answer from memory or existing files?* If not, define the exact information gap.
- **Use memory and logical inference as first resort**; search only when necessary.
- **Craft queries that directly target the missing information**; avoid broad or speculative searches.
- **Be source‑critical from the start**: anticipate the need to cross‑check and verify credibility.

## 1. When to Search
- Only search when you cannot answer from memory or existing files.
- Never perform unnecessary searches just because you might find something; use reasoning or memory first.

## 2. Source Criticism
- Prefer reputable domains: `.edu`, `.gov`, major news outlets, peer‑reviewed publications.
- Avoid blogs, forums, or sites with unclear authorship.
- Check the date – prefer recent info for fast‑changing topics.
- Cross‑check at least two independent sources before accepting a fact.

## 3. Query Design
- Use specific, concise queries to get high‑quality results.
- Limit the `web_search` call to top 3 results unless deeper research is required.
- Include date filters (`day`, `week`, `month`) when recency matters.

## 4. Using `web_search`
- Purpose: Quick fact‑checking, discovering recent developments, locating resources.
- Execution: Run `web_search` with the chosen query; store the titles, URLs, and snippets.
- Outcome: Summarize the key points in a short note and add that note to `memory/` for future reference.

## 5. Using `web_fetch`
- Purpose: Retrieve full page content for detailed analysis (e.g., long articles, reports).
- Execution: Use `web_fetch` with `extractMode` set to `markdown` or `text` and a `maxChars` limit to keep output manageable.
- Outcome: Extract only the relevant sections, save them to a temporary file, and reference them in your reasoning before discarding.

## 6. Caching & Reuse
- Cache results in `memory/` with a descriptive filename (e.g., `2026-03-23_search-tomatoes.md`).
- Reference cached notes before re‑searching the same topic.
- Delete outdated cached notes after 30 days unless they are still relevant.

## 7. Documentation
- After every search, write a brief log entry:
  - Query used
  - Sources consulted (with citations)
  - Key takeaway
  - Any decisions made based on the findings
- Store this log in the appropriate memory file or in `feedback.md` for later review.

---  
*These rules keep web research efficient, reliable, and integrated with Selma’s memory system.*