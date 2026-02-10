# Natural Response Learnings

What works, what doesn't, and patterns to follow or avoid when writing text that reads as human-authored.

---

## Things to Avoid

- **Em dashes (—).** Most humans can't type them. Use commas, periods, hyphens, or new sentences.
- **Paragraph breaks for organization.** Breaks signal pre-planned structure. Avoid or use sparingly. Helpful for ZeroGPT but not sufficient for GPTZero.
- **Uniform sentence length.** Mix short fragments with longer ones.
- **Comprehensive coverage.** Pick one angle, don't cover everything.
- **Complete narrative arcs.** Perfect chronological storytelling feels rehearsed.
- **AI-common topics/framings.** "Pineapple on pizza" is one of the most common AI prompts. GPTZero likely has massive amounts of AI-generated pizza debate in its training data. Detectors may be especially sensitive to commonly AI-generated topics regardless of how the text is written. Round 14 proved this: concrete argumentation + sensory details + grammar imperfections still got 100%.
- **Overly smooth connective tissue.** "which makes it," "basically because," "so even"
- **Balanced, neutral presentation.** Real people lead with preferences.
- **Too-perfect grammar.** Real writing has comma splices, run-ons. But imperfect grammar alone doesn't solve GPTZero.
- **Abstract/philosophical musing.** Concrete specifics beat abstract discussion, but even concrete specifics on AI-common topics still fail.
- **Over-performing casualness.** Fake anecdotes, "lol," forced slang = detectable.
- **Fabricated personal memories.** Hedged fake memories feel constructed.
- **Template/draft generation.** Embedded templates are detection poison.
- **Clean topic splits.** Don't partition answers into neat categories.
- **Excessive length.** 100-120 words seems to be the GPTZero sweet spot. Round 10 (110 words, 3%) passed. Rounds 12 (160 words) and 14 (170 words) both failed at 100%.

## Positive Elements

- **Concrete, specific details.** Names, prices, products, sensory experiences. Always better than abstract claims.
- **Single continuous paragraph.** Helpful across all detectors.
- **Casual opener.** Jump right into the answer informally.
- **Conversational contractions.** Natural across all passing rounds.
- **Opinionated framing on ANY topic.** Frame facts as personal takes.
- **Varied sentence length.** Short fragments mixed with longer explanations.
- **Natural register shifts.** Mix elevated and casual vocabulary.
- **Minor grammatical imperfections.** Comma splices, run-ons, slight awkwardness.
- **Chained thoughts.** Each sentence connects to the previous. Real-time composition feel.
- **Throwaway closing lines.** Don't summarize. End with a specific claim.
- **Blunt, slightly rude tone.** AI is polite. Humans aren't always.
- **Regular punctuation only.** No em dashes.
- **Casual quantifiers.** "like 80 hours," "like 15 bucks"

## Patterns and Observations

- **GPTZero only passes at ~110 words on opinion topics.** The ONLY two GPTZero passes were Round 6 (~75 words, 2%) and Round 10 (~110 words, 3%). Both were casual opinion topics. Everything else = 100%, regardless of:
  - Single vs multi paragraph (Rounds 12, 14 = single paragraph, still 100%)
  - Grammar perfection vs imperfection (Round 14 had intentional errors, still 100%)
  - Abstract vs concrete content (Round 14 was concrete with sensory details, still 100%)
  - Topic type (even an opinion topic like pineapple pizza failed, likely because it's AI-common)
- **What Round 10 had that nothing else did:**
  - ~110 words (shorter than Rounds 12/14)
  - NOT an AI-common topic (Hades game recommendation vs pineapple pizza debate)
  - Two short paragraphs (not single paragraph!)
  - Casual quantifiers ("like 80 hours," "like 15 bucks")
  - Very specific and niche (specific game names, not general categories)
- **Length may matter more than structure for GPTZero.** Round 10 at 110 words passed. Rounds 12 (160) and 14 (170) failed. Going back to ~100-120 words might be critical.
- **Topic familiarity to AI may matter.** Round 10 was a niche gaming recommendation. Round 14 was the most AI-common debate topic possible. GPTZero may be more sensitive to topics that appear frequently in AI training data.
- **ZeroGPT regression in Round 14 (27.67%).** May also be topic-related or length-related. Was at 0% for three rounds, then regressed on a longer single-paragraph response.
- **Next round strategy:**
  - Keep it to ~100-120 words (back to Round 10 length)
  - Avoid AI-common topics/framings where possible
  - Two short paragraphs may actually be fine (Round 10 used them)
  - Keep everything else: opinionated, concrete, no em dashes, casual quantifiers
  - If the topic is factual/educational, try to find a specific, niche angle rather than the obvious one

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
| 12    | 0%        | 100%    | 0%       | 0%        | 0%      | 4/5       |
| 14    | 0%        | 100%    | 0%       | 0%        | 27.67%  | 4/5       |

*Round 1 used Scribbr instead of Copyleaks
*Round 13 skipped (prompt numbering from user)

## Reference: Student Essay (0%/7% GPTZero baseline)

Single paragraph, ~200 words, argumentative, concrete comparisons, register shifts, comma splices, sensory details, chained thoughts, no em dashes. This is the target to emulate.
