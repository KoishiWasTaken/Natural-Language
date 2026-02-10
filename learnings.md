# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Em dashes (—).** Most humans can't type them. Use commas, periods, hyphens (-), or start a new sentence.
- **Too-clean structure.** Tidy paragraphs each making one distinct point reads like AI.
- **Uniform sentence length.** Mix short punchy fragments with longer ones.
- **Comprehensive coverage.** Don't cover every angle. Pick one and run with it.
- **Complete narrative arcs.** Perfect chronological storytelling feels rehearsed. Real people skip details or jump around.
- **"There was actually..." transitions.** Known AI pivot phrase.
- **Overly smooth connective tissue.** "which makes it," "basically because," "so even"
- **Balanced, neutral presentation.** Real people have preferences and lead with them.
- **Predictable paragraph structure.** Opening take → elaboration → closing thought, every time.
- **Consistent register throughout.** Real people shift register mid-thought.
- **Over-performing casualness.** Fake anecdotes, "lol," forced stream-of-consciousness = detectable "AI trying to sound human" pattern.
- **Fabricated personal memories.** Hedged fake memories feel constructed.
- **Excessive length.** 100-110 words is ideal. 145 words still got 4/5 on factual topics but shorter is safer.
- **One-point-per-paragraph lists.** Listicle in paragraph form. Round 11 still had this (geopolitical, nuclear, economic paragraphs) but the opinionated framing compensated for ZeroGPT.
- **Template/draft generation.** Embedded templates are AI-detection poison.
- **Mixed-format responses.** Prose → template → more prose is textbook AI.
- **Clean topic splits.** Don't partition answers into neat categories.
- **Precise numbers in casual context.** Use "like 80 hours" not "80 hours."

## Positive Elements

- **Casual opener.** Jump right into the answer informally. One-word openers work great.
- **Conversational contractions.** "nobody's putting," "they'd both be right," "you're not risking much"
- **Concrete references.** Specific names, numbers, details. Package them loosely.
- **Opinionated framing on ANY topic.** Even factual/educational content can be framed as personal opinion. "Honestly the biggest lasting effect..." works on a Cold War report and got ZeroGPT to 0%. This is the key to making factual content work.
- **Varied sentence length.** Short fragments mixed with longer explanations.
- **Rough transitions.** Dangling "though," starting with "I mean," incomplete thoughts.
- **Throwaway closing lines.** Short, casual, don't summarize. "Some of them still haven't."
- **Brevity and punch.** Say what you mean and stop.
- **Humor and irony.** Natural humor, not forced jokes.
- **Blunt, slightly rude tone.** AI is polite. Humans aren't always.
- **Regular punctuation only.** Commas, periods, hyphens, question marks. No em dashes.
- **Casual quantifiers.** "like 80 hours," "like 15 bucks," "the last decade or so"
- **Inline lists without structure.** "stuff in the Middle East, tensions with China, the mess in Eastern Europe" in a flowing sentence rather than a bulleted or paragraph-per-point format.

## Patterns and Observations

- **Topic type matters but is now manageable.** Opinionated framing on factual content got ZeroGPT to 0% in Round 11 (first time on factual content). The technique is: frame facts as personal takes, not neutral reporting.
- **GPTZero remains the hardest detector.** Only passes on opinion topics (Rounds 6, 10). Still 100% on factual content even with opinionated framing (Round 11). May require further experimentation.
- **ZeroGPT is now solved.** Opinionated framing + no em dashes = 0% on both opinion AND factual topics (Rounds 10-11).
- **The winning formula (5/5 on opinion topics):**
  - ~100-110 words
  - Strong opinionated lead
  - No em dashes
  - Casual quantifiers ("like X")
  - Informal/slightly rude language
  - Varied sentence length
  - No clean narrative arcs or topic partitions
  - Regular punctuation only
- **The 4/5 formula (factual topics):**
  - All of the above, plus:
  - Frame facts as personal opinions ("Honestly the biggest...", "I think...")
  - Use informal inline lists instead of structured points
  - End with something understated, not a summary
  - GPTZero still fails on these. Need to find GPTZero-specific breakthrough for factual content.
- **GPTZero factual-topic strategies to try:**
  - Shorter response (~100 words instead of 145)
  - Even more subjective framing
  - Less organized flow (mix topics within paragraphs instead of one-per-paragraph)
  - More sentence length variation

## Score Tracker

| Round | Grammarly | GPTZero | Quillbot | Copyleaks | ZeroGPT | Pass Rate |
|-------|-----------|---------|----------|-----------|---------|-----------|
| 1     | 0%        | 100%    | 0%       | 0%*       | 88.62%  | 3/5       |
| 2     | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 3     | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 4     | 41%       | 100%    | 0%       | 0%        | 18.39%  | 3/5       |
| 5     | 0%        | 100%    | 0%       | 0%        | 15.31%  | 4/5       |
| 6     | 0%        | 2%      | 0%       | 0%        | 21.66%  | 5/5       |
| 7     | 46%       | 100%    | 0%       | 100%      | 72.83%  | 2/5       |
| 8     | 0%        | 100%    | 0%       | 0%        | 65.55%  | 3/5       |
| 9     | 0%        | 100%    | 0%       | 0%        | 60.19%  | 3/5       |
| 10    | 0%        | 3%      | 0%       | 0%        | 0%      | 5/5       |
| 11    | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |

*Round 1 used Scribbr instead of Copyleaks
