# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Too-clean structure.** Two tidy paragraphs that each make one point, with a smooth bridge between them, reads like AI. Real people meander more.
- **Uniform sentence length.** Mixing in some short punchy fragments alongside longer ones adds texture. Round 1 sentences were all medium-length — too consistent.
- **Comprehensive coverage.** Answering a simple question by covering every angle is over-thorough. A real person would pick one angle and run with it, or be less organized about covering multiple.
- **"There was actually..." transitions.** This phrasing is a known AI pattern. Sounds like a scripted pivot to a fun fact.
- **Overly smooth connective tissue.** Phrases like "which makes it," "basically because," "so even" — every sentence flowing logically into the next without any rough edges feels machine-generated.
- **Balanced, neutral presentation.** Listing options without favoring one makes it feel like a reference article. Real people have preferences and lead with them.
- **Predictable paragraph structure.** Opening take → elaboration → closing thought is a pattern that persists across rounds. Even when content varies, the shape stays the same.
- **Consistent register throughout.** Staying at the same level of casualness the entire time might be a tell. Real people shift register mid-thought.
- **Over-performing casualness.** Leaning too hard into stream-of-consciousness, fake anecdotes, and internet-speak ("lol") creates a different but equally detectable pattern — the "AI trying to sound human" pattern. (Round 4 lesson.)
- **Fabricated personal memories.** Hedged fake memories ("I remember being maybe 8 or 9") and too-perfect narrative arcs feel constructed at the statistical level.
- **Excessive length.** Longer ≠ more human. Shorter, restrained responses (Rounds 2-3) scored best. Don't ramble to seem human.
- **One-point-per-paragraph lists.** Round 5 used four paragraphs each covering one event. This is essentially a listicle in paragraph form and may be why ZeroGPT crept up to 15.31%. Mixing multiple points within a paragraph would feel less structured.

## Positive Elements

- **Casual opener.** Informal starts that jump right into an answer consistently pass 4/5 detectors. ("Yeah, technically..." / "Oat milk, honestly." / "I mean, depends...")
- **Conversational contractions and phrasing.** "nobody's putting," "they'd both be right," "it's kind of watery" — these read naturally.
- **Concrete references and analogies.** Specific details and comparisons add personality. Package them loosely, not neatly.
- **Opinionated framing.** Stating preferences and leading with a personal take reads much more human. Works even for factual topics ("the obvious one," "doesn't get talked about enough," "deeper cut").
- **Varied sentence length.** Short fragments mixed with longer explanations consistently passes most detectors.
- **Rough transitions.** Dangling "though," starting with "I mean," incomplete thoughts with ellipsis — informality in the joints between ideas.
- **Throwaway closing lines.** Short, casual sign-offs that don't summarize or wrap up neatly.
- **Moderate length.** Sweet spot is 2-3 short paragraphs. Not curt, not a blog post.
- **Topic shapes approach.** Opinion/casual questions (Rounds 2-3) naturally score better than factual/historical ones (Round 5). Factual topics need extra effort to stay conversational and avoid informational-writing patterns.

## Patterns and Observations

- GPTZero: 100% AI across all 5 rounds. Completely unaffected by style changes. Likely uses perplexity/burstiness at the token level. May be unbeatable with prompt engineering alone.
- ZeroGPT: Sensitive to length, structure, and topic type. 0% on casual opinion topics (Rounds 2-3), creeps up on factual/historical topics (15.31% Round 5) and over-casual attempts (18.39% Round 4).
- Grammarly: Passes easily unless you over-perform casualness (41% in Round 4, 0% everywhere else).
- Quillbot and Copyleaks: Consistently 0% across all rounds. Not challenging.
- **The reliable formula (4/5):** Casually opinionated, 2-3 paragraphs, varied sentence length, rough transitions, no fake anecdotes or forced internet-speak. This has been replicated in Rounds 2, 3, and 5.
- **GPTZero ceiling:** May need to accept 4/5 as the practical limit, or investigate entirely different approaches (e.g., writing in a more formal/academic register, much shorter responses, or deliberate vocabulary shifts).

## Score Tracker

| Round | Grammarly | GPTZero | Quillbot | Copyleaks | ZeroGPT | Pass Rate |
|-------|-----------|---------|----------|-----------|---------|-----------|
| 1     | 0%        | 100%    | 0%       | 0%*       | 88.62%  | 3/5       |
| 2     | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 3     | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 4     | 41%       | 100%    | 0%       | 0%        | 18.39%  | 3/5       |
| 5     | 0%        | 100%    | 0%       | 0%        | 15.31%  | 4/5       |

*Round 1 used Scribbr instead of Copyleaks
